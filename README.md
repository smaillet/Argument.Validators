# Argument.Validators
Common annotation and argument validation support

## Examples

```C#
using namespace Ubiquity.ArgValidators
//...
public static object Load( string path, object foo, int bar )
{
    path.ValidateNotNullOrWhiteSpace( nameof( path ) );
    foo.ValidateNotNull( nameof( foo ) );
    bar.ValidateRange(3, 5, nameof( bar ) );

    //...
}
```

