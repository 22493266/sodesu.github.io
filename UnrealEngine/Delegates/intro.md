| Name | Macro | Deserializable? | Return Enable? | Payload param support? | Trigger Delegate | Bind Count | Supportedf Bind type |
| -----|:----- |:--------------: |:-------------: |:---------------------: |:---------------- |:---------: |--------------------- |
| Single |DECLARE_DELEGATE_* <br/> DECLARE_DELEGATE_RetVal_* | No | Could | Yes |1.Without return value:<br/> bool ExecuteIfBound(...)<br/>void Execute(...)<br/>2. with return value:<br/>RetValue Execute(...) | 1 | 1: Static Function:<br/>//BindStatic, CreateStatic |
