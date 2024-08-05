# Learning go

Go is a language that has for a long time been on my radar to learn and apply in my job. A recent failed venture back into product development where an untyped script language was being used, convinced me that for me to be effective in backend development, I require a strongly typed language. I was already fluent in Java, C# and TypeScript, and will definitely be approaching Golang with an object oriented mindset.

First step is to learn the basics. For that I opted for reading a book, “Go, the programming language” came to the top at Amazon Kindle, so that was the first step. Read the book. 

There are many things to like in golang. And actually none to dislike so far in the language itself.

- The data typing system is relatively simple. Basic types, arrays/slices and structs.
- The phrase “Interface” matches my understanding. One of the things that are a mental mismatch for me using TypeScript is the use of Interface to mean “Object signature” instead of “Set of callable methods on an object/class”.
- Type aliases are strongly typed. It means that I can declare a Url type that is a string, and trying to assign a Slug to it, which is also a string, will cause a compile error. This is a nice way to deal with problems stemming from primitive obsession.
- A “class” is really an interface around a struct, and how structs can be embedded rather than inherited, is a beautiful concept in my opinion. I have minimised my use of inheritance for years, and in TypeScript I prefer closure objects over class objects, so this matches my mindset nicely.
- Immutability by default. If you want references, you need to pass pointers. In languages where passing by reference is the only way, immutable structures and objects need coding gymnastics to work with. Not so in go.
- Channels and goroutines. Ahh, built in queues and synchronisation. Me like. Working with shared memory and mutexes are not a favorite of mine. This looks very nice to work with event and command based programs, which happens to be my favorite way of programming. I look forward putting this into practice.

# Testing

Test automation, including TDD, has been a special interest of mine, and therefore testable design of code. It was therefore somewhat eyebrow raising for me to see how testing with test doubles, which too many people refer to simply as mocking, was handled in the aforementioned book. 

```go
// Echo prints its command-line arguments.
package main

import (
    "flag"
    "fmt"
    "io"
    "os"
    "strings"
)

var (
    n = flag.Bool("n", false, "omit trailing newline")
    s = flag.String("s", " ", "separator")
)

var out io.Writer = os.Stdout // modified during testing

```

```go

for _, test := range tests {
        descr := fmt.Sprintf("echo(%v, %q, %q)",
            test.newline, test.sep, test.args)

        out = new(bytes.Buffer) // captured output by replacing out
        
        if err := echo(test.newline, test.sep, test.args); err != nil {
            t.Errorf("%s failed: %v", descr, err)
            continue
        }
        got := out.(*bytes.Buffer).String()
        if got != test.want {
            t.Errorf("%s = %q, want %q", descr, got, test.want)
        }
    }
```

As a long time **disciple** of Kent Beck and Robert C. Martin in software design, I am somewhat attached to the idea of dependency inversion, and in particular use of dependency injection being at the centre of testability. It follows that I am not inclined to follow this pattern from this book. I would rather do something like this:

TODO Code for IO context once refactored in project.

# Modules

There is one aspect though that caused me some doubts, especially the first time I took a look at golang some years ago. That is module system and the concept of relying on git tags for versioning modules is not entirely robust. It means putting a lot of trust in module authors not to mess with their git tags once published, or put in a countermeasure to verify sources (VERIFY: Are module source checksums stored by default ?).

I am guessing that the authors wanted to avoid the [npmjs.com](http://npmjs.com) pattern for some reason.

Use the language to do something productive.


# Mux is a nice router. 

The example tests leave a thing or two to be desired. I like to test as much of the "wiring" as well, not only the handlers
in isolation.
