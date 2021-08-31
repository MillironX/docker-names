# Docker Names

An implementation of [docker-names](https://github.com/moby/moby/blob/master/pkg/namesgenerator/names-generator.go) in TypeScript. Forked from <https://github.com/criblio/docker-names>.

## Changes

1. Added more names of scientists related to
   - chemical engineering
   - animal breeding
   - rumen science
   - among others...
2. Changed the delimiter to an underscore when adding extra data (date or number)
3. Added an identifier that starts with a date (useful where identifiers have to be sorted chronologically).

## Usage

Maybe this stuff will still work? :shrug: I just replaced everything with my name and code, but I personally transpile to JavaScript rather than use TypeScript directly.

### Generate Name

```typescript
import {generateName} from '@millironx/docker-names'

const dockerName = generateName();

console.log(dockerName);

//Outputs goofy-panini
```

### Generate Name With Number

```typescript
import {generateNameWithNumber} from '@millironx/docker-names'

const dockerName = generateNameWithNumber();

console.log(dockerName);

//Outputs goofy-panini_4
```

### Generate Name With Date

```typescript
import {generateNameWithDate} from '@millironx/docker-names'

const dockerName = generateNameWithDate();

console.log(dockerName);

//Outputs 20210720_goofy-panini
```

## Words

The words can also be imported from the package if need be.

```typescript
import {left,right} from '@millironx/docker-names'

console.log(left);

//Outputs [admiring,adoring, etc...]

console.log(right)

//Outputs [albattani,allen, etc...]
```
