# Hypercolor HTTP Errors

## Table of Contents
  - [Introduction](#introduction)
  - [Installation](#installation)
  - [Usage](#usage)
  - [License](LICENSE)
  - [More Information](#more-information)
    - [Project Repository](#project-repository)
    - [Organization Repository](#organization-repository)
    
## Introduction
This tool is used by the team at Hypercolor to provide consistent HTTP Error formatting between services for a given project.

## Installation
  - NPM 
    - `npm i @hypercolor/http-errors`
  - Yarn 
    - `yarn add @hypercolor/http-errors`
  
## Usage
Example:
```typescript
import { NotFoundError } from '@hypercolor/http-errors';

export class Service {
    public async findSomething(id: number) {
        const found = await this.findSomething(id);
        if (!found) {
            throw new NotFoundError('Something not found with ID: ' + id);
        }
        return found;
    }
}

```
## More Information

#### [Project Repository](https://github.com/hypercolor/http-errors)

#### [Organization Repository](https://github.com/hypercolor/)
