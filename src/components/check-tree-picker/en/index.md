# CheckTreePicker

CheckTreePicker are supported in multiple selectors for multiple selection of complex data structures.

- `<CheckTreePicker>` The selector component supports Checkbox on the TreePicker node for multiple selection.

## Usage

```js
import { CheckTreePicker } from 'rsuite';
```

## Examples

<!--{demo}-->

## Props

### <CheckTreePicker>

| Property              | Type `(Default)`                                                                       | Description                                                 |
| --------------------- | -------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| appearance            | enum: 'default', 'subtle' `('default')`                                                | Set picker appearence                                       |
| block                 | boolean                                                                                | Blocking an entire row                                      |
| cascade               | boolean                                                                                | whether cascade select                                      |
| childKey              | string `('children')`                                                                  | set children key in data                                    |
| cleanable             | boolean `(true)`                                                                       | whether the selected value can be cleared                   |
| container             | HTMLElement or (() => HTMLElement)                                                     | Sets the rendering container                                |
| countable             | boolean `(true)`                                                                       | whether display counts of checkItems                        |
| data \*               | Array&lt;[DataItemType](#types)&gt;                                                    | tree data                                                   |
| defaultExpandAll      | boolean                                                                                | expand all tree node                                        |
| defaultValue          | string[]                                                                               | (UnControlled) default values of the selected tree node     |
| disabled              | boolean                                                                                | whether disabled                                            |
| disabledItemValues    | string[]                                                                               | values of disabled tree node                                |
| expandAll             | boolean                                                                                | Expand or unExpand all nodes(Controlled)                    |
| labelKey              | string `('label')`                                                                     | set label key in data                                       |
| menuClassName         | string                                                                                 | className for Menu                                          |
| menuStyle             | React.CSSProperties                                                                    | style for Menu                                              |
| onChange              | (values:string[])=>void                                                                | callback fired when value change                            |
| onClose               | ()=>void                                                                               | callback fired when close component                         |
| onExpand              | (activeNode:[DataItemType](#types),layer:number, concat:(data, children)=>Array)=>void | callback fired when tree node expand state changed          |
| onOpen                | ()=>void                                                                               | callback fired when open component                          |
| onSearch              | (searchKeyword:string, event)=>void                                                    | callback fired when search                                  |
| onSelect              | (activeNode:[DataItemType](#types), layer:number, values:string[])=>void               | callback fired when tree node is selected                   |
| placeholder           | React.Node `('Select')`                                                                |                                                             |
| placement             | enum: [Placement](#types) `('bottomLeft')`                                             | Placement of component                                      |
| renderExtraFooter     | ()=>React.Node                                                                         | custom render extra footer                                  |
| renderMenu            | (menu:React.Node)=>React.Node                                                          | Customizing the Rendering Menu list                         |
| renderTreeIcon        | (nodeData:Array&lt;Object&gt;)=>React.Node                                             | custom render the icon of tree node                         |
| renderTreeNode        | (nodeData:Array&lt;[DataItemType](#types)&gt;)=>React.Node                             | custom render tree node                                     |
| renderValue           | (values:any[], checkedItems:any[],selectedElement:React.Node)=>React.Node              | custom render placeholder                                   |
| seasrchable           | boolean `(true)`                                                                       | whether display search input box                            |
| toggleComponentClass  | React.ElementType `('a')`                                                              | You can use a custom element for this component             |
| uncheckableItemValues | string[]                                                                               | Set the option value for the check box not to be rendered   |
| value                 | string[]                                                                               | (Controlled) specifies the values of the selected tree node |
| valueKey              | string `('value')`                                                                     | set value key in data                                       |


## Related Components

- [`<CheckTree>`](./check-tree)
- [`<Tree>`](./tree)
- [`<TreePicker>`](./tree-picker)
