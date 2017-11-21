<div align="center">
  <img src="https://raw.githubusercontent.com/typectrl/ngx-github-buttons/master/src/assets/share.png" width="300" alt="Angular GitHub Buttons">
  <br>
  <h1>ngx-github-buttons</h1>
  <a href="https://www.npmjs.com/package/@ctrl/ngx-github-buttons">
    <img src="https://img.shields.io/npm/v/@ctrl/ngx-github-buttons.svg" alt="npm">
  </a> 
  <a href="https://travis-ci.org/TypeCtrl/ngx-github-buttons">
    <img src="https://travis-ci.org/TypeCtrl/ngx-github-buttons.svg?branch=master" alt="travis"></a> 
</div>
<br>
<br>

> GitHub buttons without the iframe, rewritten in Angular.  

__Choose from two styles__:  
- ntkme: https://buttons.github.io/  
- mdo: https://ghbtns.com/  

### Demo
https://typectrl.github.io/ngx-github-buttons/  

### Install
```sh
npm i @ctrl/ngx-github-buttons
```

### Use
Import the component
```ts
import { NtkmeButtonModule } from '@ctrl/ngx-github-buttons';
// or
import { MdoButtonModule } from '@ctrl/ngx-github-buttons';
``` 
Use the component
```html
<ntkme-github-button
  user="angular"
  repo="angular"
  >
</ntkme-github-button>
```  
or  
```html
<mdo-github-button
  user="angular"
  repo="angular"
  >
</mdo-github-button>
```  

### API
| Input        | Type    | default | Description                                                        |
| ------------ | ------- | ------- | ------------------------------------------------------------------ |
| user         | string  |         | user or org                                                        |
| repo         | string  |         | repository name                                                    |
| type         | string  | `star`  | `star`, `follow`, `watch`, `fork`. ntkme only: `issue`, `download` |
| count        | boolean | `false` | show count of stars, issues, followers etc.                        |
| size         | string  | `'none'`| `'large'` for a bigger size button                                 |
| standardIcon | boolean | `false` | ntkme only: use the github logo instead of other icons             |


### License
Compilicated. This project is MIT licensed, but each set of buttons have their own license which must be respected.  
The mdo buttons are Licensed [Apache 2](https://github.com/mdo/github-buttons/blob/master/LICENSE.md)  
The ntkme buttons are Licensed [BSD 2-clause](https://github.com/ntkme/github-buttons/blob/master/LICENSE.md)  
