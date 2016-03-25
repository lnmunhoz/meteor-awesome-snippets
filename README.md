# meteor-awesome-snippets
A collection of snippets that makes working with meteor easy!

## HTML

### [>] {{> myTemplate}}
```handlebars
{{> ${1:myTemplate}}}
```

### [af] autoForm
```handlebars
{{#autoForm id="${1}" collection="${2}" type="${3}"}}
	${4}
{{/autoForm}}
```

### [afm] autoform (type="method")
```handlebars
{{#autoForm id="${1}" collection="${2}" type="method" meteormethod="${3}"}}
	${4}
{{/autoForm}}
```

### [afmu] aufotorm (type="method-update")
```handlebars
{{#autoForm id="${1}" collection="${2}" type="method-update" meteormethod="${3}" doc=${4}}}
	${5}
{{/autoForm}}
```

### [each] each block
```handlebars
{{#each ${1:helper}}} 
	${2}
{{/each}}
```

### [eache] each else block
```handlebars
{{#each ${1:helper}}} 
	${2}

	{{else}}

{{/each}}
```

### [if] if block
```handlebars
{{#if ${1:helper}}} 
	${2}
{{/if}}
```

### [ife] if else block
```handlebars
{{#if ${1:helper}}} 
	${2}

	{{else}}
	
{{/if}}
```

### [ifetsr] if else block Template.subscriptionsReady
```handlebars
{{#if Template.subscriptionsReady}}
	${1}

	{{else}}

{{/if}}
```

### [iftsr] if block Template.subscriptionsReady
```handlebars
{{#if Template.subscriptionsReady}}
	${1}
{{/if}}
```

### [t] template
```handlebars
<template name="${1}">
	${2}
</template>
```

### [tsr] Template.subscriptionsReady
```handlebars
Template.subscriptionsReady
```

### [with] with block
```handlebars
{{#with ${1:helper}}} 
	${2}
{{/with}}
```
 
## JavaScript

### [cf] Collection.find
```js
${1:Collection}.find({
	${2:key}: ${3:value}
});
```

### [cfo] Collection.findOne
```js
${1:Collection}.findOne({
	${2:key}: ${3:value}
});
```

### [cu] Collection.update
```js
${1:Collection}.update({
	${2:key}: ${3:value}
}, {
	${4:modifier}
});
```

### [mp] Meteor.publish
```js
Meteor.publish('${1}', function(${2:params}){
	return ${3:Collection}.find({${4}});	
});
```

### [mpc] Meteor.publishComposite
```js
Meteor.publishComposite('${1}', function(${2:params}) {
	return {
		find() {
			return ${3:Collection}.find({${4}});
		},
		children: [{
			find(${5:topLevelDocument}) {
				return ${6:Collection}.find({${7}});
			}
		}]
	};
});
```

### [t] Template
```js
Template
```

### [te] Template.myTemplate.events
```js
Template.${1:myTemplate}.events({
	'${2:event} ${3:selector}': function (event, template) {
		${4}
	}
});
```

### [th] Template.myTemplate.helpers
```js
Template.${1:myTemplate}.helpers({
	${2:helper}() {
		${3}
	}
});
```

### [ti] Template.instance()
```js
Template.instance()
```

### [tid] Tempalte.instance().data
```js
Template.instance().data
```

### [toc] Template.myTemplate.onCreated 
```js
Template.${1:myTemplate}.onCreated(function() {
  ${2}
});
```

### [tod] Template.myTemplate.onDestroyed
```js
Template.${1:myTemplate}.onDestroyed(function() {
  ${2}
});
```

### [tor] Template.myTemplate.onRendered
```js
Template.${1:myTemplate}.onRendered(function() {
  ${2}
});
```

## Contributing
Please send your PR!











