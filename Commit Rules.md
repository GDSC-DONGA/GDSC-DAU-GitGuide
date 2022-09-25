# Need for Commit message

- Communication with the team members
- Convenient tracking of past records
- You can check the progress related to the issue while writing the issue together

# How to write a commit message

```
Type: Subject

Body

Footer
```

## What mean type?

- `Feat` - Add new function
- `Fix` - Bug fixes
- `Build` - Modify build related files
- `Ci` - Modify CI(Continuity Integrated) related settings
- `Docs` - Documentation (add, edit, delete documents)
- `Style` - Style (code format, add semicolon: if no change in business logic)
- `Refactor` - code refactoring
- `Test` - Test (Add, modify, delete test code: if there is no change in business logic)
- `Chore` - Miscellaneous changes (fix build scripts, etc.)

## How to writing subject?

- Titles must be no longer than `50 characters`, and do not include periods.
- Write the `commit type` together in the title.
- `Do not use the past` tense and write in imperative.
- The title and body are `separated` by a single space.
- `The first letter `of the title must be `capitalized`.
- The title or body text should `include the issue number` (if any)  

**Ex) Type - Subject**
~~~
Feat: New recognition function added
~~~

## How to writing body?
- `As this is optional`, there is no need to write body content in every commit.
- Do not exceed `72 characters` on a line.
- Write according to `what and why` rather than how.
- It is used not only as a `description`, but also when writing the reason for the `commit`.

**Ex) Body**
~~~
New recognition function added
    -Reader.Js:  Added recognition function due to user requirements
~~~

## How to writing Footer?
- `It's optional`, so you don't need to put a footer on every commit.
- Used to create an `issue tracker ID`.
- `Resolution`: Used when resolving issues
- `RELATED`: Issue number related to that commit
- `Note`: Use if you have issues to refer to

**Ex) Footer**

~~~
Resolutuin : #issues number
~~~

## Hands - On
~~~
Fead: New recognition function added

New recognition function added
    -Reader.Js: Added recognition function due to user requirements

Resolutuin : #1234
~~~

## Tip, Auto closing of issues with commit message
> Git-hub is equipped with a function that `automatically closes` an issue when a reserved `keyword` is used when writing English in a commit message.  
Reserved words can be used `anywhere` in the commit message.

### Hands - On
~~~
Keyword #issues number
~~~

### Auto closing keyword list

- close
- closes
- closed
- fix
- fixes
- fixed
- resolve
- resolves
- resolved

# Let's settle a culture that fits the Commit message Rule together.

Writer - jh park  
Email - jhparkintlot@gmail.com  
Instagram - jh_parkland  
[Homepage](https://www.jhpark.org/)
