# Boolean values

!!! tip inline end "Mixing `true`, `false`, `yes`, `no`, and their cases"
    That works but just don't, makes playbooks very hard to read

| Value | What can represent it in Ansible? |
| - | - |
| `True` | Boolean `True`, case-insensitive: `True`, `true` |
| | Special `yes` value, case-insensitive: `Yes`, `yes`
| | Positive numbers: `1`, `2`, `8472365`, etc. |
| | Non-empty strings: `'test'`, `"0"`, `'Ansible'`, etc. |
| `False` | Boolean `False`, case-insensitive: `False`, `false` |
| | Special `no` value, case-insensitive: `No`, `no` |
| | `0` and negative numbers: `0`, `-1`, `-8472365`, etc. |
| | Empty strings: `''`, `""`
