# api documentation for  [ng-annotate (v1.2.1)](https://github.com/olov/ng-annotate#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ng-annotate.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ng-annotate) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ng-annotate.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ng-annotate)
#### add, remove and rebuild angularjs dependency injection annotations

[![NPM](https://nodei.co/npm/ng-annotate.png?downloads=true)](https://www.npmjs.com/package/ng-annotate)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ng-annotate/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ng-annotate_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ng-annotate/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ng-annotate/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ng-annotate/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Olov Lassus",
        "email": "olov.lassus@gmail.com"
    },
    "bin": {
        "ng-annotate": "./build/es5/ng-annotate"
    },
    "bugs": {
        "url": "https://github.com/olov/ng-annotate/issues"
    },
    "dependencies": {
        "acorn": "~2.6.4",
        "alter": "~0.2.0",
        "convert-source-map": "~1.1.2",
        "optimist": "~0.6.1",
        "ordered-ast-traverse": "~1.1.1",
        "simple-fmt": "~0.1.0",
        "simple-is": "~0.2.0",
        "source-map": "~0.5.3",
        "stable": "~0.1.5",
        "stringmap": "~0.2.2",
        "stringset": "~0.2.1",
        "tryor": "~0.1.2"
    },
    "description": "add, remove and rebuild angularjs dependency injection annotations",
    "devDependencies": {
        "coffee-script": "~1.10.0",
        "defs": "~1.1.1",
        "diff": "~2.2.1",
        "find-line-column": "~0.5.2"
    },
    "directories": {},
    "dist": {
        "shasum": "eb8bc1a6731c70d08af6b02c3eaf1a6e3fb9e6bb",
        "tarball": "https://registry.npmjs.org/ng-annotate/-/ng-annotate-1.2.1.tgz"
    },
    "homepage": "https://github.com/olov/ng-annotate#readme",
    "keywords": [
        "angular",
        "angularjs",
        "di",
        "dependency",
        "injection",
        "annotate",
        "annotation",
        "annotations",
        "transformation"
    ],
    "license": "MIT",
    "main": "build/es5/ng-annotate-main.js",
    "maintainers": [
        {
            "name": "olov",
            "email": "olov.lassus@gmail.com"
        }
    ],
    "name": "ng-annotate",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/olov/ng-annotate.git"
    },
    "scripts": {
        "test": "node --harmony run-tests"
    },
    "version": "1.2.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ng-annotate](#apidoc.module.ng-annotate)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>lut (ast, src)](#apidoc.element.ng-annotate.lut)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>pos_to_linecolumn (str)](#apidoc.element.ng-annotate.pos_to_linecolumn)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>scope (args)](#apidoc.element.ng-annotate.scope)
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>angular_dashboard_framework
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>lut.prototype
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>nginject
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>pos_to_linecolumn.prototype
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>scope.prototype
1.  object <span class="apidocSignatureSpan">ng-annotate.</span>scopetools

#### [module ng-annotate.angular_dashboard_framework](#apidoc.module.ng-annotate.angular_dashboard_framework)
1.  [function <span class="apidocSignatureSpan">ng-annotate.angular_dashboard_framework.</span>init (_ctx)](#apidoc.element.ng-annotate.angular_dashboard_framework.init)
1.  [function <span class="apidocSignatureSpan">ng-annotate.angular_dashboard_framework.</span>match (node)](#apidoc.element.ng-annotate.angular_dashboard_framework.match)

#### [module ng-annotate.lut](#apidoc.module.ng-annotate.lut)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>lut (ast, src)](#apidoc.element.ng-annotate.lut.lut)

#### [module ng-annotate.lut.prototype](#apidoc.module.ng-annotate.lut.prototype)
1.  [function <span class="apidocSignatureSpan">ng-annotate.lut.prototype.</span>findNodeBeforePos (pos)](#apidoc.element.ng-annotate.lut.prototype.findNodeBeforePos)
1.  [function <span class="apidocSignatureSpan">ng-annotate.lut.prototype.</span>findNodeFromPos (pos)](#apidoc.element.ng-annotate.lut.prototype.findNodeFromPos)

#### [module ng-annotate.nginject](#apidoc.module.ng-annotate.nginject)
1.  [function <span class="apidocSignatureSpan">ng-annotate.nginject.</span>inspectComments (ctx)](#apidoc.element.ng-annotate.nginject.inspectComments)
1.  [function <span class="apidocSignatureSpan">ng-annotate.nginject.</span>inspectNode (node, ctx)](#apidoc.element.ng-annotate.nginject.inspectNode)

#### [module ng-annotate.pos_to_linecolumn](#apidoc.module.ng-annotate.pos_to_linecolumn)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>pos_to_linecolumn (str)](#apidoc.element.ng-annotate.pos_to_linecolumn.pos_to_linecolumn)

#### [module ng-annotate.pos_to_linecolumn.prototype](#apidoc.module.ng-annotate.pos_to_linecolumn.prototype)
1.  [function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toColumn (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toColumn)
1.  [function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toLine (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLine)
1.  [function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toLineColumn (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLineColumn)

#### [module ng-annotate.scope](#apidoc.module.ng-annotate.scope)
1.  [function <span class="apidocSignatureSpan">ng-annotate.</span>scope (args)](#apidoc.element.ng-annotate.scope.scope)

#### [module ng-annotate.scope.prototype](#apidoc.module.ng-annotate.scope.prototype)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>add (name, kind, node, referableFromPos)](#apidoc.element.ng-annotate.scope.prototype.add)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>closestHoistScope ()](#apidoc.element.ng-annotate.scope.prototype.closestHoistScope)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>doesPropagate (name)](#apidoc.element.ng-annotate.scope.prototype.doesPropagate)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getFromPos (name)](#apidoc.element.ng-annotate.scope.prototype.getFromPos)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getKind (name)](#apidoc.element.ng-annotate.scope.prototype.getKind)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getNode (name)](#apidoc.element.ng-annotate.scope.prototype.getNode)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>hasOwn (name)](#apidoc.element.ng-annotate.scope.prototype.hasOwn)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>lookup (name)](#apidoc.element.ng-annotate.scope.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>markPropagates (name)](#apidoc.element.ng-annotate.scope.prototype.markPropagates)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>print (indent)](#apidoc.element.ng-annotate.scope.prototype.print)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>remove (name)](#apidoc.element.ng-annotate.scope.prototype.remove)

#### [module ng-annotate.scopetools](#apidoc.module.ng-annotate.scopetools)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scopetools.</span>isReference (node)](#apidoc.element.ng-annotate.scopetools.isReference)
1.  [function <span class="apidocSignatureSpan">ng-annotate.scopetools.</span>setupScopeAndReferences (root)](#apidoc.element.ng-annotate.scopetools.setupScopeAndReferences)



# <a name="apidoc.module.ng-annotate"></a>[module ng-annotate](#apidoc.module.ng-annotate)

#### <a name="apidoc.element.ng-annotate.lut"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>lut (ast, src)](#apidoc.element.ng-annotate.lut)
- description and source-code
```javascript
function Lut(ast, src) {
    assert(this instanceof Lut);

    const sparseBegins = new Array(src.length);
    const begins = [];
    const sparseEnds = new Array(src.length);
    const ends = [];
    let p = 0;
    const t0 = Date.now();
    traverse(ast, {pre: function(node) {
        //        assert (node.range[0] >= p);
        if (node.type === "Program") {
            return;
        }
        p = node.range[0];
        if (!sparseBegins[p]) {
            sparseBegins[p] = node;
        }
        p = node.range[1];
        if (!sparseEnds[p]) {
            sparseEnds[p] = node;
        }
    }});
    for (let i in sparseBegins) {
        begins.push(sparseBegins[i]);
    }
    for (let i in sparseEnds) {
        ends.push(sparseEnds[i]);
    }
    const t1 = Date.now();
    //    console.error(t1-t0)

    // begins and ends are compact arrays with nodes,
    // sorted on node.range[0/1] (unique)
    this.begins = begins;
    this.ends = ends;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ng-annotate.pos_to_linecolumn"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>pos_to_linecolumn (str)](#apidoc.element.ng-annotate.pos_to_linecolumn)
- description and source-code
```javascript
function PosToLineColumn(str) {
    if (!(this instanceof PosToLineColumn)) {
        throw new Error("PosToLineColumn requires new");
    }
    str = String(str);

    const newlines = [];
    let pos = -1;
    while ((pos = str.indexOf("\n", pos + 1)) >= 0) {
        newlines.push(pos);
    }

    let line = 1;
    let column = 0;
    const columns = [];
    const lines = [];
    let i;
    let j = 0;
    for (i = 0; i < str.length; i++) {
        columns[i] = column;
        lines[i] = line;

        if (i === newlines[j]) {
            ++j;
            ++line;
            column = 0;
        } else {
            ++column;
        }
    }

    // add extra entry to support pos === str.length
    columns[i] = column;
    lines[i] = line;

    this.len = str.length;
    this.columns = columns;
    this.lines = lines;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ng-annotate.scope"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>scope (args)](#apidoc.element.ng-annotate.scope)
- description and source-code
```javascript
function Scope(args) {
    assert(is.someof(args.kind, ["hoist", "block", "catch-block"]));
    assert(is.object(args.node));
    assert(args.parent === null || is.object(args.parent));

    // kind === "hoist": function scopes, program scope, injected globals
    // kind === "block": ES6 block scopes
    // kind === "catch-block": catch block scopes
    this.kind = args.kind;

    // the AST node the block corresponds to
    this.node = args.node;

    // parent scope
    this.parent = args.parent;

    // children scopes for easier traversal (populated internally)
    this.children = [];

    // scope declarations. decls[variable_name] = {
    //     kind: "fun" for functions,
    //           "param" for function parameters,
    //           "caught" for catch parameter
    //           "var",
    //           "const",
    //           "let"
    //     node: the AST node the declaration corresponds to
    //     from: source code index from which it is visible at earliest
    //           (only stored for "const", "let" [and "var"] nodes)
    // }
    this.decls = stringmap();

    // names of all variables declared outside this hoist scope but
    // referenced in this scope (immediately or in child).
    // only stored on hoist scopes for efficiency
    // (because we currently generate lots of empty block scopes)
    this.propagates = (this.kind === "hoist" ? stringset() : null);

    // scopes register themselves with their parents for easier traversal
    if (this.parent) {
        this.parent.children.push(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ng-annotate.angular_dashboard_framework"></a>[module ng-annotate.angular_dashboard_framework](#apidoc.module.ng-annotate.angular_dashboard_framework)

#### <a name="apidoc.element.ng-annotate.angular_dashboard_framework.init"></a>[function <span class="apidocSignatureSpan">ng-annotate.angular_dashboard_framework.</span>init (_ctx)](#apidoc.element.ng-annotate.angular_dashboard_framework.init)
- description and source-code
```javascript
init = function (_ctx) {
    ctx = _ctx;
}
```
- example usage
```shell
...
    }
    return false;
}
const matchPluginsOrNull = (plugins.length === 0 ? null : matchPlugins);

ngInject.inspectComments(ctx);
plugins.forEach(function(plugin) {
    plugin.init(ctx);
});

traverse(ast, {pre: function(node) {
    ngInject.inspectNode(node, ctx);

}, post: function(node) {
    ctx.nodePositions.push(node.loc.start);
...
```

#### <a name="apidoc.element.ng-annotate.angular_dashboard_framework.match"></a>[function <span class="apidocSignatureSpan">ng-annotate.angular_dashboard_framework.</span>match (node)](#apidoc.element.ng-annotate.angular_dashboard_framework.match)
- description and source-code
```javascript
match = function (node) {
    // dashboardProvider.widget("name", {
    //   ...
    //   controller: function($scope) {},
    //   resolve: {f: function($scope) {}, ..}
    // })

    const callee = node.callee;
    if (!callee) {
        return false;
    }

    const obj = callee.object;
    if (!obj) {
        return false;
    }

    // identifier or expression
    if (!(obj.$chained === 1 || (obj.type === "Identifier" && obj.name === "dashboardProvider"))) {
        return false;
    }

    node.$chained = 1;

    const method = callee.property; // identifier
    if (method.name !== "widget") {
        return false;
    }

    const args = node.arguments;
    if (args.length !== 2) {
        return false;
    }

    const configArg = ctx.last(args);
    if (configArg.type !== "ObjectExpression") {
        return false;
    }

    const props = configArg.properties;
    const res = [
        ctx.matchProp("controller", props)
    ];
    // {resolve: ..}
    res.push.apply(res, ctx.matchResolve(props));

    // edit: {controller: function(), resolve: {}, apply: function()}
    const edit = ctx.matchProp('edit', props);
    if (edit && edit.type === "ObjectExpression") {
        const editProps = edit.properties;
        res.push(ctx.matchProp('controller', editProps));
        res.push(ctx.matchProp('apply', editProps));
        res.push.apply(res, ctx.matchResolve(editProps));
    }

    const filteredRes = res.filter(Boolean);
    return (filteredRes.length === 0 ? false : filteredRes);
}
```
- example usage
```shell
...
    return allOptionals[optional];
});

const plugins = [].concat(optionalsPlugins, options.plugin || []);

function matchPlugins(node, isMethodCall) {
    for (let i = 0; i < plugins.length; i++) {
        const res = plugins[i].match(node, isMethodCall);
        if (res) {
            return res;
        }
    }
    return false;
}
const matchPluginsOrNull = (plugins.length === 0 ? null : matchPlugins);
...
```



# <a name="apidoc.module.ng-annotate.lut"></a>[module ng-annotate.lut](#apidoc.module.ng-annotate.lut)

#### <a name="apidoc.element.ng-annotate.lut.lut"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>lut (ast, src)](#apidoc.element.ng-annotate.lut.lut)
- description and source-code
```javascript
function Lut(ast, src) {
    assert(this instanceof Lut);

    const sparseBegins = new Array(src.length);
    const begins = [];
    const sparseEnds = new Array(src.length);
    const ends = [];
    let p = 0;
    const t0 = Date.now();
    traverse(ast, {pre: function(node) {
        //        assert (node.range[0] >= p);
        if (node.type === "Program") {
            return;
        }
        p = node.range[0];
        if (!sparseBegins[p]) {
            sparseBegins[p] = node;
        }
        p = node.range[1];
        if (!sparseEnds[p]) {
            sparseEnds[p] = node;
        }
    }});
    for (let i in sparseBegins) {
        begins.push(sparseBegins[i]);
    }
    for (let i in sparseEnds) {
        ends.push(sparseEnds[i]);
    }
    const t1 = Date.now();
    //    console.error(t1-t0)

    // begins and ends are compact arrays with nodes,
    // sorted on node.range[0/1] (unique)
    this.begins = begins;
    this.ends = ends;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ng-annotate.lut.prototype"></a>[module ng-annotate.lut.prototype](#apidoc.module.ng-annotate.lut.prototype)

#### <a name="apidoc.element.ng-annotate.lut.prototype.findNodeBeforePos"></a>[function <span class="apidocSignatureSpan">ng-annotate.lut.prototype.</span>findNodeBeforePos (pos)](#apidoc.element.ng-annotate.lut.prototype.findNodeBeforePos)
- description and source-code
```javascript
function findNodeBeforePos(pos) {
    const lut = this.ends;
    assert(is.finitenumber(pos) && pos >= 0);

    let left = 0;
    let right = lut.length - 1;
    while (left < right) {
        const mid = Math.ceil((left + right) / 2);
        assert(mid >= 0 && mid < lut.length);
        if (pos < lut[mid].range[1]) {
            right = mid - 1;
        }
        else {
            left = mid;
        }
    }
    if (left > right) {
        assert(lut[0].range[1] > pos);
        return null;
    }

    const found = left;
    const foundPos = lut[found].range[1];
    if(foundPos > pos) {
        return null;
    }
    if (found <= lut.length - 2) {
        const nextPos = lut[found + 1].range[1];
        assert(nextPos > pos);
    }

    return lut[found];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ng-annotate.lut.prototype.findNodeFromPos"></a>[function <span class="apidocSignatureSpan">ng-annotate.lut.prototype.</span>findNodeFromPos (pos)](#apidoc.element.ng-annotate.lut.prototype.findNodeFromPos)
- description and source-code
```javascript
function findNodeFromPos(pos) {
    const lut = this.begins;
    assert(is.finitenumber(pos) && pos >= 0);

    let left = 0;
    let right = lut.length - 1;
    while (left < right) {
        const mid = Math.floor((left + right) / 2);
        assert(mid >= 0 && mid < lut.length);
        if (pos > lut[mid].range[0]) {
            left = mid + 1;
        }
        else {
            right = mid;
        }
    }
    if (left > right) {
        assert(last(lut).range[0] < pos);
        return null;
    }

    const found = left;
    const foundPos = lut[found].range[0];
    assert(foundPos >= pos);
    if (found >= 1) {
        const prevPos = lut[found - 1].range[0];
        assert(prevPos < pos);
    }

    return lut[found];
}
```
- example usage
```shell
...
    stats.parser_parse_t1 = Date.now();
} catch(e) {
    return {
        errors: ["error: couldn't process source due to parse error", e.message],
    };
}

// append a dummy-node to ast so that lut.findNodeFromPos(lastPos) returns something
ast.body.push({
    type: "DebuggerStatement",
    range: [ast.range[1], ast.range[1]],
    loc: {
        start: ast.loc.end,
        end: ast.loc.end
    }
...
```



# <a name="apidoc.module.ng-annotate.nginject"></a>[module ng-annotate.nginject](#apidoc.module.ng-annotate.nginject)

#### <a name="apidoc.element.ng-annotate.nginject.inspectComments"></a>[function <span class="apidocSignatureSpan">ng-annotate.nginject.</span>inspectComments (ctx)](#apidoc.element.ng-annotate.nginject.inspectComments)
- description and source-code
```javascript
function inspectComments(ctx) {
    const comments = ctx.comments;
    for (let i = 0; i < comments.length; i++) {
        const comment = comments[i];
        const yesPos = comment.value.indexOf("@ngInject");
        const noPos = (yesPos === -1 ? comment.value.indexOf("@ngNoInject") : -1);
        if (yesPos === -1 && noPos === -1) {
            continue;
        }

        const target = ctx.lut.findNodeFromPos(comment.range[1]);
        if (!target) {
            continue;
        }

        addSuspect(target, ctx, noPos >= 0);
    }
}
```
- example usage
```shell
...
            return res;
        }
    }
    return false;
}
const matchPluginsOrNull = (plugins.length === 0 ? null : matchPlugins);

ngInject.inspectComments(ctx);
plugins.forEach(function(plugin) {
    plugin.init(ctx);
});

traverse(ast, {pre: function(node) {
    ngInject.inspectNode(node, ctx);
...
```

#### <a name="apidoc.element.ng-annotate.nginject.inspectNode"></a>[function <span class="apidocSignatureSpan">ng-annotate.nginject.</span>inspectNode (node, ctx)](#apidoc.element.ng-annotate.nginject.inspectNode)
- description and source-code
```javascript
function inspectNode(node, ctx) {
    if (node.type === "CallExpression") {
        inspectCallExpression(node, ctx);
    } else if (node.type === "FunctionExpression" || node.type === "FunctionDeclaration") {
        inspectFunction(node, ctx);
    }
}
```
- example usage
```shell
...

ngInject.inspectComments(ctx);
plugins.forEach(function(plugin) {
    plugin.init(ctx);
});

traverse(ast, {pre: function(node) {
    ngInject.inspectNode(node, ctx);

}, post: function(node) {
    ctx.nodePositions.push(node.loc.start);
    let targets = match(node, ctx, matchPluginsOrNull);
    if (!targets) {
        return;
    }
...
```



# <a name="apidoc.module.ng-annotate.pos_to_linecolumn"></a>[module ng-annotate.pos_to_linecolumn](#apidoc.module.ng-annotate.pos_to_linecolumn)

#### <a name="apidoc.element.ng-annotate.pos_to_linecolumn.pos_to_linecolumn"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>pos_to_linecolumn (str)](#apidoc.element.ng-annotate.pos_to_linecolumn.pos_to_linecolumn)
- description and source-code
```javascript
function PosToLineColumn(str) {
    if (!(this instanceof PosToLineColumn)) {
        throw new Error("PosToLineColumn requires new");
    }
    str = String(str);

    const newlines = [];
    let pos = -1;
    while ((pos = str.indexOf("\n", pos + 1)) >= 0) {
        newlines.push(pos);
    }

    let line = 1;
    let column = 0;
    const columns = [];
    const lines = [];
    let i;
    let j = 0;
    for (i = 0; i < str.length; i++) {
        columns[i] = column;
        lines[i] = line;

        if (i === newlines[j]) {
            ++j;
            ++line;
            column = 0;
        } else {
            ++column;
        }
    }

    // add extra entry to support pos === str.length
    columns[i] = column;
    lines[i] = line;

    this.len = str.length;
    this.columns = columns;
    this.lines = lines;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ng-annotate.pos_to_linecolumn.prototype"></a>[module ng-annotate.pos_to_linecolumn.prototype](#apidoc.module.ng-annotate.pos_to_linecolumn.prototype)

#### <a name="apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toColumn"></a>[function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toColumn (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toColumn)
- description and source-code
```javascript
toColumn = function (pos) {
    assert(pos >= 0 && pos <= this.len);
    return this.columns[pos];
}
```
- example usage
```shell
...
assert(pos >= 0 && pos <= this.len);
return this.columns[pos];
};

PosToLineColumn.prototype.toLineColumn = function(pos) {
return {
    line: this.toLine(pos),
    column: this.toColumn(pos),
};
};


/*
const tst = "asdf\n" +
"abc\n" +
...
```

#### <a name="apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLine"></a>[function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toLine (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLine)
- description and source-code
```javascript
toLine = function (pos) {
    assert(pos >= 0 && pos <= this.len);
    return this.lines[pos];
}
```
- example usage
```shell
...
PosToLineColumn.prototype.toColumn = function(pos) {
    assert(pos >= 0 && pos <= this.len);
    return this.columns[pos];
};

PosToLineColumn.prototype.toLineColumn = function(pos) {
    return {
        line: this.toLine(pos),
        column: this.toColumn(pos),
    };
};


/*
const tst = "asdf\n" +
...
```

#### <a name="apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLineColumn"></a>[function <span class="apidocSignatureSpan">ng-annotate.pos_to_linecolumn.prototype.</span>toLineColumn (pos)](#apidoc.element.ng-annotate.pos_to_linecolumn.prototype.toLineColumn)
- description and source-code
```javascript
toLineColumn = function (pos) {
    return {
        line: this.toLine(pos),
        column: this.toColumn(pos),
    };
}
```
- example usage
```shell
...
const tst = "asdf\n" +
    "abc\n" +
    "d\n" +
    "\n\n" +
    "efghi a\r\n" +
    "x";
const instance = new PosToLineColumn(tst);
console.dir(instance.toLineColumn(0));
console.dir(instance.toLineColumn(tst.length));
*/
...
```



# <a name="apidoc.module.ng-annotate.scope"></a>[module ng-annotate.scope](#apidoc.module.ng-annotate.scope)

#### <a name="apidoc.element.ng-annotate.scope.scope"></a>[function <span class="apidocSignatureSpan">ng-annotate.</span>scope (args)](#apidoc.element.ng-annotate.scope.scope)
- description and source-code
```javascript
function Scope(args) {
    assert(is.someof(args.kind, ["hoist", "block", "catch-block"]));
    assert(is.object(args.node));
    assert(args.parent === null || is.object(args.parent));

    // kind === "hoist": function scopes, program scope, injected globals
    // kind === "block": ES6 block scopes
    // kind === "catch-block": catch block scopes
    this.kind = args.kind;

    // the AST node the block corresponds to
    this.node = args.node;

    // parent scope
    this.parent = args.parent;

    // children scopes for easier traversal (populated internally)
    this.children = [];

    // scope declarations. decls[variable_name] = {
    //     kind: "fun" for functions,
    //           "param" for function parameters,
    //           "caught" for catch parameter
    //           "var",
    //           "const",
    //           "let"
    //     node: the AST node the declaration corresponds to
    //     from: source code index from which it is visible at earliest
    //           (only stored for "const", "let" [and "var"] nodes)
    // }
    this.decls = stringmap();

    // names of all variables declared outside this hoist scope but
    // referenced in this scope (immediately or in child).
    // only stored on hoist scopes for efficiency
    // (because we currently generate lots of empty block scopes)
    this.propagates = (this.kind === "hoist" ? stringset() : null);

    // scopes register themselves with their parents for easier traversal
    if (this.parent) {
        this.parent.children.push(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ng-annotate.scope.prototype"></a>[module ng-annotate.scope.prototype](#apidoc.module.ng-annotate.scope.prototype)

#### <a name="apidoc.element.ng-annotate.scope.prototype.add"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>add (name, kind, node, referableFromPos)](#apidoc.element.ng-annotate.scope.prototype.add)
- description and source-code
```javascript
add = function (name, kind, node, referableFromPos) {
    assert(is.someof(kind, ["fun", "param", "var", "caught", "const", "let"]));

    function isConstLet(kind) {
        return is.someof(kind, ["const", "let"]);
    }

    let scope = this;

    // search nearest hoist-scope for fun, param and var's
    // const, let and caught variables go directly in the scope (which may be hoist, block or catch-block)
    if (is.someof(kind, ["fun", "param", "var"])) {
        while (scope.kind !== "hoist") {
//            if (scope.decls.has(name) && isConstLet(scope.decls.get(name).kind)) { // could be caught
//                return error(getline(node), "{0} is already declared", name);
//            }
            scope = scope.parent;
        }
    }
    // name exists in scope and either new or existing kind is const|let => error
//    if (scope.decls.has(name) && (isConstLet(scope.decls.get(name).kind) || isConstLet(kind))) {
//        return error(getline(node), "{0} is already declared", name);
//    }

    const declaration = {
        kind: kind,
        node: node,
    };
    if (referableFromPos) {
        assert(is.someof(kind, ["var", "const", "let"]));
        declaration.from = referableFromPos;
    }
    scope.decls.set(name, declaration);
}
```
- example usage
```shell
...
};

Scope.prototype.doesPropagate = function(name) {
return this.propagates.has(name);
};

Scope.prototype.markPropagates = function(name) {
this.propagates.add(name);
};

Scope.prototype.closestHoistScope = function() {
let scope = this;
while (scope.kind !== "hoist") {
    scope = scope.parent;
}
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.closestHoistScope"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>closestHoistScope ()](#apidoc.element.ng-annotate.scope.prototype.closestHoistScope)
- description and source-code
```javascript
closestHoistScope = function () {
    let scope = this;
    while (scope.kind !== "hoist") {
        scope = scope.parent;
    }
    return scope;
}
```
- example usage
```shell
...
    // This is used to mark "taint" the name since adding a new variable in the scope,
    // with a propagated name, would change the meaning of the existing references.
    //
    // catch(e) is special because even though e is a variable in its own scope,
    // we want to make sure that catch(e){let e} is never transformed to
    // catch(e){var e} (but rather var e$0). For that reason we taint the use of e
    // in the closest hoist-scope, i.e. where var e$0 belongs.
    node.$scope.closestHoistScope().markPropagates(identifier.name);

} else if (node.type === "Program") {
    // Top-level program is a scope
    // There's no block-scope under it
    node.$scope = new Scope({
        kind: "hoist",
        node: node,
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.doesPropagate"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>doesPropagate (name)](#apidoc.element.ng-annotate.scope.prototype.doesPropagate)
- description and source-code
```javascript
doesPropagate = function (name) {
    return this.propagates.has(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.getFromPos"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getFromPos (name)](#apidoc.element.ng-annotate.scope.prototype.getFromPos)
- description and source-code
```javascript
getFromPos = function (name) {
    assert(is.string(name));
    const decl = this.decls.get(name);
    return decl ? decl.from : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.getKind"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getKind (name)](#apidoc.element.ng-annotate.scope.prototype.getKind)
- description and source-code
```javascript
getKind = function (name) {
    assert(is.string(name));
    const decl = this.decls.get(name);
    return decl ? decl.kind : null;
}
```
- example usage
```shell
...

const scope = node.$scope.lookup(node.name);
if (!scope) {
    return null;
}

const parent = scope.getNode(node.name).$parent;
const kind = scope.getKind(node.name);
if (!parent) {
    return null;
}
const ptype = parent.type;

if (is.someof(kind, ["const", "let", "var"])) {
    assert(ptype === "VariableDeclarator");
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.getNode"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>getNode (name)](#apidoc.element.ng-annotate.scope.prototype.getNode)
- description and source-code
```javascript
getNode = function (name) {
    assert(is.string(name));
    const decl = this.decls.get(name);
    return decl ? decl.node : null;
}
```
- example usage
```shell
...
}

const scope = node.$scope.lookup(node.name);
if (!scope) {
    return null;
}

const parent = scope.getNode(node.name).$parent;
const kind = scope.getKind(node.name);
if (!parent) {
    return null;
}
const ptype = parent.type;

if (is.someof(kind, ["const", "let", "var"])) {
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.hasOwn"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>hasOwn (name)](#apidoc.element.ng-annotate.scope.prototype.hasOwn)
- description and source-code
```javascript
hasOwn = function (name) {
    return this.decls.has(name);
}
```
- example usage
```shell
...
}

function createTopScope(programScope) {
function inject(obj) {
    for (let name in obj) {
        const writeable = obj[name];
        const kind = (writeable ? "var" : "const");
        if (topScope.hasOwn(name)) {
            topScope.remove(name);
        }
        topScope.add(name, kind, {loc: {start: {line: -1}}}, -1);
    }
}

const topScope = new Scope({
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.lookup"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>lookup (name)](#apidoc.element.ng-annotate.scope.prototype.lookup)
- description and source-code
```javascript
lookup = function (name) {
    for (let scope = this; scope; scope = scope.parent) {
        if (scope.decls.has(name)) {
            return scope;
        } else if (scope.kind === "hoist") {
            scope.propagates.add(name);
        }
    }
    return null;
}
```
- example usage
```shell
...
}

function followReference(node) {
if (!scopeTools.isReference(node)) {
    return null;
}

const scope = node.$scope.lookup(node.name);
if (!scope) {
    return null;
}

const parent = scope.getNode(node.name).$parent;
const kind = scope.getKind(node.name);
if (!parent) {
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.markPropagates"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>markPropagates (name)](#apidoc.element.ng-annotate.scope.prototype.markPropagates)
- description and source-code
```javascript
markPropagates = function (name) {
    this.propagates.add(name);
}
```
- example usage
```shell
...
    // This is used to mark "taint" the name since adding a new variable in the scope,
    // with a propagated name, would change the meaning of the existing references.
    //
    // catch(e) is special because even though e is a variable in its own scope,
    // we want to make sure that catch(e){let e} is never transformed to
    // catch(e){var e} (but rather var e$0). For that reason we taint the use of e
    // in the closest hoist-scope, i.e. where var e$0 belongs.
    node.$scope.closestHoistScope().markPropagates(identifier.name);

} else if (node.type === "Program") {
    // Top-level program is a scope
    // There's no block-scope under it
    node.$scope = new Scope({
        kind: "hoist",
        node: node,
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.print"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>print (indent)](#apidoc.element.ng-annotate.scope.prototype.print)
- description and source-code
```javascript
print = function (indent) {
    indent = indent || 0;
    const scope = this;
    const names = this.decls.keys().map(function(name) {
        return fmt("{0} [{1}]", name, scope.decls.get(name).kind);
    }).join(", ");
    const propagates = this.propagates ? this.propagates.items().join(", ") : "";
    console.log(fmt("{0}{1}: {2}. propagates: {3}", fmt.repeat(" ", indent), this.node.type, names, propagates));
    this.children.forEach(function(c) {
        c.print(indent + 2);
    });
}
```
- example usage
```shell
...
const scope = this;
const names = this.decls.keys().map(function(name) {
    return fmt("{0} [{1}]", name, scope.decls.get(name).kind);
}).join(", ");
const propagates = this.propagates ? this.propagates.items().join(", ") : "";
console.log(fmt("{0}{1}: {2}. propagates: {3}", fmt.repeat(" ", indent), this.node.type, names, propagates));
this.children.forEach(function(c) {
    c.print(indent + 2);
});
};

Scope.prototype.add = function(name, kind, node, referableFromPos) {
assert(is.someof(kind, ["fun", "param", "var", "caught", "const", "let"]));

function isConstLet(kind) {
...
```

#### <a name="apidoc.element.ng-annotate.scope.prototype.remove"></a>[function <span class="apidocSignatureSpan">ng-annotate.scope.prototype.</span>remove (name)](#apidoc.element.ng-annotate.scope.prototype.remove)
- description and source-code
```javascript
remove = function (name) {
    return this.decls.remove(name);
}
```
- example usage
```shell
...
};

Scope.prototype.hasOwn = function(name) {
    return this.decls.has(name);
};

Scope.prototype.remove = function(name) {
    return this.decls.remove(name);
};

Scope.prototype.doesPropagate = function(name) {
    return this.propagates.has(name);
};

Scope.prototype.markPropagates = function(name) {
...
```



# <a name="apidoc.module.ng-annotate.scopetools"></a>[module ng-annotate.scopetools](#apidoc.module.ng-annotate.scopetools)

#### <a name="apidoc.element.ng-annotate.scopetools.isReference"></a>[function <span class="apidocSignatureSpan">ng-annotate.scopetools.</span>isReference (node)](#apidoc.element.ng-annotate.scopetools.isReference)
- description and source-code
```javascript
function isReference(node) {
    const parent = node.$parent;
    return node.$refToScope ||
        node.type === "Identifier" &&
            !(parent.type === "VariableDeclarator" && parent.id === node) && // var|let|const $
            !(parent.type === "MemberExpression" && parent.computed === false && parent.property === node) && // obj.$
            !(parent.type === "Property" && parent.key === node) && // {$: ...}
            !(parent.type === "LabeledStatement" && parent.label === node) && // $: ...
            !(parent.type === "CatchClause" && parent.param === node) && // catch($)
            !(isFunction(parent) && parent.id === node) && // function $(..
            !(isFunction(parent) && is.someof(node, parent.params)) && // function f($)..
            true;
}
```
- example usage
```shell
...
        target.$seen = val;
        return true;
    });
}
}

function followReference(node) {
if (!scopeTools.isReference(node)) {
    return null;
}

const scope = node.$scope.lookup(node.name);
if (!scope) {
    return null;
}
...
```

#### <a name="apidoc.element.ng-annotate.scopetools.setupScopeAndReferences"></a>[function <span class="apidocSignatureSpan">ng-annotate.scopetools.</span>setupScopeAndReferences (root)](#apidoc.element.ng-annotate.scopetools.setupScopeAndReferences)
- description and source-code
```javascript
function setupScopeAndReferences(root) {
    traverse(root, {pre: createScopes});
    createTopScope(root.$scope);
}
```
- example usage
```shell
...

// Position information for all nodes in the AST,
// used for sourcemap generation
const nodePositions = [];

const lut = new Lut(ast, src);

scopeTools.setupScopeAndReferences(ast);

const ctx = {
    mode: mode,
    quot: quot,
    src: src,
    srcForRange: function(range) {
        return src.slice(range[0], range[1]);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
