# OluFooter

A simple footer that accepts a string of text and list of links

## Example

<Demo componentName="examples-olufooter-doc" />

## Usage
<SourceCode>
<<< @/docs/.vuepress/components/examples/olufooter-doc.vue
</SourceCode>

## Source Code

<SourceCode>
<<< @/src/components/OluFooter/OluFooter.vue
</SourceCode>

## Slots

### default

The string of text to display in the footer

## Props

| Prop     | Type     | Required  | Description |
|----------|----------|-----------|-------------|
| links    | Array    | False     | Array of objects with fields `url` and `label` |
