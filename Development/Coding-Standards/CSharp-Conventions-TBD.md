1. Properties capitilized
`public Guid EvaluationId {get; set;}`

2. Private members prefixed with '_'
`private IEvaluationService _evaluationService;`

3. Curly braces in their own line for namespaces and classes
`namespace Malue.App.UI.MAUI`
`{`
&nbsp;&nbsp;&nbsp;&nbsp;`public class Test`
&nbsp;&nbsp;&nbsp;&nbsp;`{`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`//implmentation`
&nbsp;&nbsp;&nbsp;&nbsp;`}`
`}`
4. Curly braces in the same line for if else, for/foreach, switch
`if(condition) {`
&nbsp;&nbsp;&nbsp;&nbsp;`//Do something`
`}`
5. Always use Curly braces for if else even if it contains 1 line of code
`if(condition) {`
&nbsp;&nbsp;&nbsp;&nbsp;`//Do something`
`}`
instead of
`if(condition)`
&nbsp;&nbsp;&nbsp;&nbsp;`//Do something`
6. Spaces instead of Tabs
Set Tab size to 4 spaces in Visual Studio
![image.png](/.attachments/image-7b081416-2dee-4f3e-936c-f9dffbcdc0bb.png)

7. Braces for Namespace:
`namespace Data`
`{`
&nbsp;&nbsp;&nbsp;&nbsp;`//classes and code`
`}`
instead of 
`namespace Data;`
8. Don't use short aliases for primitive types
use 
`Boolean, String, Int32 and etc`
instead of
`bool, string, int and etc`
