# C# Coding Conventions

**Every developer must follow this guidelines to keep project's code clear and easy maintainable for a long time.**
Our style guide relies on standard C# guidelines. For anything not specified below, use _ref.pdf_ attached document.

## Whitespace

- Do use 2 spaces (no tabs), 4 spaces for line continuations
- Do use 100 characters line margin (120 very exceptional)
- Do add blank line **at the end of file**, blank line after **attributed** class members
- Do use blank lines before and after **condition/loop** statements

## Braces and parenthesis

- Do **vertically** align curly brackets to conform original C# style
- Do use space before and after **operators**

## Naming

- Do use **MixedCase** for class names, method names and constants
- Do use **camelCase** for method arguments, class variables and local variables
- Do use **noun** or noun phrases to name a class
- Do prefix interfaces with the letter **I**. Interface names are **noun** (phrases) or adjectives
- Do try to fit class/method names into **24** characters
- Do use singular names for enums

- **Do not** use CAPS for commonly used abbreviations such as *Id, Xml, Ftp, Uri*
- **Do not** use underscores in any kind of identifiers
- **Do not** suffix enum names with Enum

## Code Structure

- Do organize namespaces with to conform **folder** structure. Exception: corporate prefix e.g. **MintFrogs.ProjectX**
- Do use implicit type **var** for local variable declarations
- Do use **predefined** type names instead of system type names like *Int16, Single, UInt64*, etc
- Do name source files according to their main classes

- Do declare all class members in following order:
```csharp
public class Clazz
{
    public static Constant
    public const Constant

    private static Constant
    private const Constant   

    private memberVarialble
    protected memberVarialble

    public static Method

    public Clazz() { }

    public Property {get; set;}

    public Method

    protected Method    
}
```

## Comments

- All comments must be in **English**
- All files must be prefixed with appropriate **license** header

## Unity

- Do name **MonoBehaviour** derived classes with Behaviour postfix
- **Do not** use coroutines for asynchronous computations
