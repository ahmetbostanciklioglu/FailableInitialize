# FailableInitialize



**Failable initialize:**
```
class FailableClass {
    var property: String
    
    init?(property: String) {
        if property.count == 12 {
            self.property = property
        }else {
            return nil
        }
    }
}
let objectOfFailableClass = FailableClass(property: "1234")
```

```
var stringProperty = "False"
let transformStringToBool = Bool(stringProperty) //nil
/*MARK: if the value of stringProperty is "true" or "false" Bool(stringProperty) will convert string to optional bool value, else value of transformStringToBool will be nil.
*/
```
