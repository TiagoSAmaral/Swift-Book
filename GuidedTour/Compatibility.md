 Version Compatibility

Version Compatibility
=====================

This book describes Swift 5.1, the default version of Swift that’s included in Xcode 11. You can use Xcode 11 to build targets that are written in either Swift 5.1, Swift 4.2, or Swift 4.

When you use Xcode 11 to build Swift 4 and Swift 4.2 code, most Swift 5.1 functionality is available. That said, the following changes are available only to code that uses Swift 5.1 or later:

*   Functions that return an opaque type require the Swift 5.1 runtime.
    
*   The `try?` expression doesn’t introduce an extra level of optionality to expressions that already return optionals.
    
*   Large integer literal initialization expressions are inferred to be of the correct integer type. For example, `UInt64(0xffff_ffff_ffff_ffff)` evaluates to the correct value rather than overflowing.
    

A target written in Swift 5.1 can depend on a target that’s written in Swift 4.2 or Swift 4, and vice versa. This means, if you have a large project that’s divided into multiple frameworks, you can migrate your code from Swift 4 to Swift 5.1 one framework at a time.