# chan

Chan is a likeable CLI tool used for writing and maintaining a CHANGELOG empowering the user to use a coloquial/friendly style. See more here: http://keepachangelog.com/

____

## **Disclaimer**:

Tool at early stage, the API will change until we get the kind of usage style we have in mind. You are noticed. :warning:

## Getting started

Development stage:

```bash
git clone it

npm run build && npm link
```

## API/Usage

```bash
chan <CATEGORY> <MSG>
```

Where:

- ```CATEGORY```: It is the category verb in past tense. Categories can be: added, removed, fixed, updated, changed, etc.
- ```MSG```: It is your message describing what changed according to the category selected.

## Parser

The following represents the parsed CHANGELOG as an object with custom functionality. This is the extension point, transformations are built using this data representation.

```
[ Root ]
    [ Release ]
        [ *Category ]
            [ *Msg ]
                [ Commit-Link ]
                [ Issue-Link ]

* = one or more
```

___

By **GEUT** - 2016
