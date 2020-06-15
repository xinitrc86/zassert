# zassert
Assert abstract class for ABAP test classes. 
Allows you to write cleaner tests.

From:
```
    cl_abap_unit_assert=>assert_equals(
        exp = "A"
        act = "B"
        msg = "C"
    ).
```

To:
```
    assert_equals(
        exp = "A"
        act = "B"
        msg = "C"
    ).
```

## Usage

Inherit it in your your test classes.

```
class ltc_aunit_result_adapter definition
  for testing
  duration short
  risk level harmless
  inheriting from zcl_assert.

```

Use any of the methods available in cl_abap_unit_assert.


## Installation
Just clone it or import the zip with [ABAPGit](https://github.com/larshp/abapGit).
