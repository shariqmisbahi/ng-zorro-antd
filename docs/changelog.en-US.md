---
order: 13
title: Change Log
toc: false
timeline: true
---
`ng-zorro-antd` strictly follows [Semantic Versioning 2.0.0](https://semver.org).

#### Release Schedule

* Weekly release: patch version at the end of every week for routine bugfix (anytime for urgent bugfix).
* Monthly release: minor version at the end of every month for new features.
* Major version release is not included in this schedule for breaking change and new features.

---

## 11.0.0

`2020-12-21`


## Highlights

### RTL Support

Set the dir attribute on the document body or html tag.
```html
<html dir="rtl"></html>
```

Or use Angular CDK bidi module for bi-directional.

```typescript
import {BidiModule} from '@angular/cdk/bidi';
```

Super thanks to [@saeedrahimi](https://github.com/saeedrahimi), [@hdm91](https://github.com/hdm91), [@HDaghash](https://github.com/HDaghash), [@hmdnikoo](https://github.com/hmdnikoo) for contributing this!

### New Image component

Used to handle progressive loading of images; failure fallback, and preview of image(s).

Super thanks to [@stygian-desolator](https://github.com/stygian-desolator) for contributing this!

### New Graph experimental component

Support customized multi-level graph rendering.

### New Tree View component

The previous Tree already contains many common features, and to handle more customizable scenarios we developed a more basic Tree View component with higher ability of customization and better control over performance.

### New built-in Aliyun theme

```less
@import "~ng-zorro-antd/ng-zorro-antd.aliyun.less";
```

### Bug Fixes

* **tree:** fix tree styles ([#6198](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6198)) ([a481a15](https://github.com/NG-ZORRO/ng-zorro-antd/commit/a481a156278047472e1324b87df896b37246a0ed))
* **button:** only warn about deprecated value when used ([#6193](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6193)) ([40c644a](https://github.com/NG-ZORRO/ng-zorro-antd/commit/40c644aa8fe92ccfaf26220a872b0995874b2569)), closes [#6191](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6191) [#6187](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6187)
* **i18n:** fix Ukrainian i18n file ([#6236](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6236)) ([551c7a2](https://github.com/NG-ZORRO/ng-zorro-antd/commit/551c7a24c1ae0cec9f15f61bcaa12b9057de4bd0))
* **image:** fix RTL direction and props ([#6227](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6227)) ([3978e0f](https://github.com/NG-ZORRO/ng-zorro-antd/commit/3978e0f48c3924fdbfda54e69438ea794b29a8ec))
* **list:** fix template rendering order ([#6232](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6232)) ([4324011](https://github.com/NG-ZORRO/ng-zorro-antd/commit/43240113c66c583e806f87b84b669a6ddb1faffe)), closes [#6229](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6229)
* **modal:** fix `nzOkDanger` in confirm mode ([#6214](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6214)) ([ebe2869](https://github.com/NG-ZORRO/ng-zorro-antd/commit/ebe2869d1b9459a8e02e3993d8a93483fa531f62))
* **select:** fix XSS vulnerabilities ([#6222](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6222)) ([a393b89](https://github.com/NG-ZORRO/ng-zorro-antd/commit/a393b89bf82eece5b0586592d709629865b27b3a)), closes [#6209](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6209)
* **table:** false nzFrontPagination hides pagination ([#6201](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6201)) ([8029ef4](https://github.com/NG-ZORRO/ng-zorro-antd/commit/8029ef47d6eeaf43aa5875f8a8034205dc9c69bb)), closes [#6196](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6196)
* **time-picker:** placeholder not update with i18n changes ([#6069](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6069)) ([f34840b](https://github.com/NG-ZORRO/ng-zorro-antd/commit/f34840bf2a4c5eb2d2facba0fa00068f6fa2bd5e))


### Features

* **all:** add RTL support to all ng-zorro-antd ([#4703](https://github.com/NG-ZORRO/ng-zorro-antd/issues/4703)) ([860dfed](https://github.com/NG-ZORRO/ng-zorro-antd/commit/860dfeddcf02fc7e775615244827cb224d1aa8be)), closes [#4704](https://github.com/NG-ZORRO/ng-zorro-antd/issues/4704) [#1762](https://github.com/NG-ZORRO/ng-zorro-antd/issues/1762) [#5261](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5261)
* **date-picker:** add `nzShowNow` ([#6160](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6160)) ([99e3117](https://github.com/NG-ZORRO/ng-zorro-antd/commit/99e3117b70853c0aa4f6b4f475b031734840f10f)), closes [#6146](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6146)
* **graph:** add graph component ([#6053](https://github.com/NG-ZORRO/ng-zorro-antd/pull/6053)) ([e69303f](https://github.com/NG-ZORRO/ng-zorro-antd/commit/e69303f828132cb62263867abe8afefc600f15f6))
* **image:** add image component ([#6154](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6154)) ([83dfdf9](https://github.com/NG-ZORRO/ng-zorro-antd/commit/83dfdf97b5a716e1cc9424d645dfc6713fe4ba64))
* **tree-view:** add tree-view component ([#6161](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6161)) ([05d58de](https://github.com/NG-ZORRO/ng-zorro-antd/commit/05d58de21f8a3e4d3e2bf4d4333de95a2c71e1ed)), closes [#5976](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5976) [#5809](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5809) [#5739](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5739) [#5736](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5736) [#5519](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5519) [#5446](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5446) [#5152](https://github.com/NG-ZORRO/ng-zorro-antd/issues/5152) [#4694](https://github.com/NG-ZORRO/ng-zorro-antd/issues/4694) [#4472](https://github.com/NG-ZORRO/ng-zorro-antd/issues/4472) [#3832](https://github.com/NG-ZORRO/ng-zorro-antd/issues/3832) [#2785](https://github.com/NG-ZORRO/ng-zorro-antd/issues/2785) [#2744](https://github.com/NG-ZORRO/ng-zorro-antd/issues/2744) [#6199](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6199)
* **schematics:** make ng-add schematics chainable ([#6203](https://github.com/NG-ZORRO/ng-zorro-antd/issues/6203)) ([d1e76f3](https://github.com/NG-ZORRO/ng-zorro-antd/commit/d1e76f3d8d41b0e3b9f01887e4805ff43f48d0fa))

### BREAKING CHANGES

**date-picker**
- `[nzMode]` does not support `NzDateMode[]` type any more, please adjust it manually.

**modal**
- `[nzGetContainer]` has been removed, please remove it manually.
- `open` method in `NzModalRef` has been removed, please remove it manually.

**tabs**
- `[nzShowPagination]` input has been removed, please remove it manually.
- `(nzOnPrevClick)` output has been removed, please remove it manually.
- `(nzOnNextClick)` output has been removed, please remove it manually.
- `a[nz-tab-link]` selector has been removed, please use `ng-template[nzTabLink] > a[nz-tab-link]` instead.

## Old Versions

All releases notes can be found [here](https://github.com/NG-ZORRO/ng-zorro-antd/releases)
