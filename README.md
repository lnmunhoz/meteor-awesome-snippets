# meteor-awesome-snippets

## HTML

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

 
## JavaScript


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












