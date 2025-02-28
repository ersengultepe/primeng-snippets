# PrimeNG Quickly for VS Code

**Created for PrimeNG Quickly release**

This extension for Visual Studio Code includes a lot of primeNG elements that allow you to quickly add snippets in Typescript and HTML files if you install PrimeNG in your Angular applications.
Currently snippets for **form**, **button**, **data** and **panel** elements are available, but will be updated frequently for other primeNG elements. 
Stay tuned !!!

> Panel Elements Added 

See the [CHANGELOG](CHANGELOG.md) for the latest changes

## Download

Download the extension from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=ErsenGultepe.primeng-quikcly).

## Usage

Type part of a snippet, press `tab`, and the snippet unfolds.

Alternatively, press `Ctrl`+`Space` (Windows, Linux) or `Cmd`+`Space` (macOS) to activate snippets from within the editor.

## Features

- **Quick Access**: Quickly add PrimeNG components to your project.
- **Ease of Use**: Snippets automatically generate the basic usage of components.
- **Up-to-Date PrimeNG Support**: Compatible with the latest versions of PrimeNG.

## Requirements

- **Visual Studio Code**: Version 1.10.0 or higher.
- **Angular Project**: An Angular project with PrimeNG installed (snippets will work, but PrimeNG dependency is required for components to render).

## Installing PrimeNG

To use the extension, you need to install PrimeNG in your project. Follow these steps:

1. Open a terminal and navigate to your project directory.
2. Run the following command to install PrimeNG, Prime Themes, PrimeIcons and PrimeFlex(optional) :

### Using npm
```sh
npm install primeng @primeng/themes primeicons primeflex
```

### Using yarn

```sh
yarn add primeng @primeng/themes primeicons primeflex
```
### Using pnpm

```sh
pnpm add primeng @primeng/themes primeicons primeflex
```

# CSS Import

Import the following files into style.css or style.scss

@import "primeflex/primeflex.css";
@import "primeicons/primeicons.css";


## Configuring PrimeNG

To configure PrimeNG with animations and a theme, update your application configuration as follows:

```typescript
import { ApplicationConfig } from '@angular/core';
import { provideAnimationsAsync } from '@angular/platform-browser/animations/async';
import { providePrimeNG } from 'primeng/config';
import Aura from '@primeng/themes/aura';

export const appConfig: ApplicationConfig = {
    providers: [
        provideAnimationsAsync(),
        providePrimeNG({
            theme: {
                preset: Aura
            }
        })
    ]
};
```

## Available PrimeNG Components in Snippets

`Form Components`
AutoComplete, CascadeSelect, Checkbox, ColorPicker, DatePicker, Editor, FloatLabel, IconField, InputGroup, InputMask, InputNumber, InputOTP, InputText, KeyFilter, Knob, ListBox, MultiSelect, Password, RadioButton, Rating, Select, SelectButton, Slider, TextArea, ToggleButton, ToggleSwitch, TreeSelect, 

`Button Components`
Button, SpeedDial, SplitButton

`Data Components`
DataView, OrderList, OrgChart, Paginator, PickList, Table, TimeLine, Tree, TreeTable, VirtualScroller

### Snippets for the following components will be added very soon.
*Panel, Overlay, File, Menu, Chart, Messages, Media, Misc*


## Extension Installation

1. Install Visual Studio Code 1.10.0 or higher
1. Launch Code
1. From the command palette `Ctrl`-`Shift`-`P` (Windows, Linux) or `Cmd`-`Shift`-`P` (OSX)
1. Select `Install Extension`
1. Choose the extension
1. Reload Visual Studio Code

## Credits

This plugin was created with artificial intelligence support. Thanks to the free services of the following AI language models, the laborious work is made much easier.

- [Le Chat - Mistral AI](https://chat.mistral.ai/)
- [Grok 3](https://grok.com/)
- [ChatGpt](https://chatgpt.com/)
- [Deepseek](https://chat.deepseek.com/)
- [Phind](https://www.phind.com/)

Plugin logo created by Canva

- [Canva - Free Online AI Image Generator](https://www.canva.com/ai-image-generator/)

![Logo](images/logo.png)



| Snippet                                    | Purpose                                                              |
|--------------------------------------------|----------------------------------------------------------------------|
| p-autocomplete-import                      | Imports PrimeNG AutoCompleteModule in TypeScript                     |
| p-autocomplete-component                   | PrimeNG AutoComplete component snippet                               |
| p-autocomplete-dropdown-component         | PrimeNG AutoComplete Dropdown component snippet                      |
| p-autocomplete-reactive-form-component     | PrimeNG AutoComplete Reactive Form component snippet                 |
| p-button-import                            | Imports PrimeNG ButtonModule in TypeScript                           |
| p-button-basic                             | PrimeNG Button component snippet                                     |
| p-button-badge                             | PrimeNG Button with Badge snippet                                    |
| p-button-badge-icon                        | PrimeNG Button with Badge and Icon snippet                           |
| p-button-contrast                          | PrimeNG Button with Contrast style snippet                           |
| p-button-contrast-outlined                 | PrimeNG Button with Contrast Outlined style snippet                  |
| p-button-contrast-raised                   | PrimeNG Button with Contrast Raised style snippet                    |
| p-button-contrast-rounded                  | PrimeNG Button with Contrast Rounded style snippet                   |
| p-button-danger                            | PrimeNG Button with Danger style snippet                             |
| p-button-danger-outlined                   | PrimeNG Button with Danger Outlined style snippet                    |
| p-button-danger-raised                     | PrimeNG Button with Danger Raised style snippet                      |
| p-button-danger-rounded                    | PrimeNG Button with Danger Rounded style snippet                     |
| p-button-danger-text                       | PrimeNG Button with Danger Text style snippet                        |
| p-button-danger-text-raised                | PrimeNG Button with Danger Text Raised style snippet                 |
| p-button-disabled                          | PrimeNG Button in Disabled state snippet                             |
| p-button-group                             | PrimeNG Button Group component snippet                               |
| p-button-help                              | PrimeNG Button with Help style snippet                               |
| p-button-help-outlined                     | PrimeNG Button with Help Outlined style snippet                      |
| p-button-help-raised                       | PrimeNG Button with Help Raised style snippet                        |
| p-button-help-rounded                      | PrimeNG Button with Help Rounded style snippet                       |
| p-button-help-text                         | PrimeNG Button with Help Text style snippet                          |
| p-button-help-text-raised                  | PrimeNG Button with Help Text Raised style snippet                   |
| p-button-icon                              | PrimeNG Button with Icon snippet                                     |
| p-button-icon-bell-rounded-outlined-warn   | PrimeNG Button with Bell Icon, Rounded Outlined Warn style snippet   |
| p-button-icon-bell-rounded-text-raised-warn| PrimeNG Button with Bell Icon, Rounded Text Raised Warn style snippet|
| p-button-icon-bell-rounded-text-warn       | PrimeNG Button with Bell Icon, Rounded Text Warn style snippet       |
| p-button-icon-bell-rounded-warn            | PrimeNG Button with Bell Icon, Rounded Warn style snippet            |
| p-button-icon-bell-warn                    | PrimeNG Button with Bell Icon, Warn style snippet                    |
| p-button-icon-bookmark-rounded-outlined-secondary | PrimeNG Button with Bookmark Icon, Rounded Outlined Secondary style snippet |
| p-button-icon-bookmark-rounded-secondary   | PrimeNG Button with Bookmark Icon, Rounded Secondary style snippet   |
| p-button-icon-bookmark-rounded-text-raised-secondary | PrimeNG Button with Bookmark Icon, Rounded Text Raised Secondary style snippet |
| p-button-icon-bookmark-rounded-text-secondary | PrimeNG Button with Bookmark Icon, Rounded Text Secondary style snippet |
| p-button-icon-bookmark-secondary           | PrimeNG Button with Bookmark Icon, Secondary style snippet           |
| p-button-icon-check                        | PrimeNG Button with Check Icon snippet                               |
| p-button-icon-check-rounded                | PrimeNG Button with Check Icon, Rounded style snippet                |
| p-button-icon-check-rounded-outlined       | PrimeNG Button with Check Icon, Rounded Outlined style snippet       |
| p-button-icon-check-rounded-text           | PrimeNG Button with Check Icon, Rounded Text style snippet           |
| p-button-icon-check-rounded-text-raised    | PrimeNG Button with Check Icon, Rounded Text Raised style snippet    |
| p-button-icon-heart-help                   | PrimeNG Button with Heart Icon, Help style snippet                   |
| p-button-icon-heart-rounded-help           | PrimeNG Button with Heart Icon, Rounded Help style snippet           |
| p-button-icon-heart-rounded-outlined-help  | PrimeNG Button with Heart Icon, Rounded Outlined Help style snippet  |
| p-button-icon-heart-rounded-text-help      | PrimeNG Button with Heart Icon, Rounded Text Help style snippet      |
| p-button-icon-heart-rounded-text-raised-help | PrimeNG Button with Heart Icon, Rounded Text Raised Help style snippet |
| p-button-icon-search-rounded-outlined-success | PrimeNG Button with Search Icon, Rounded Outlined Success style snippet |
| p-button-icon-search-rounded-success       | PrimeNG Button with Search Icon, Rounded Success style snippet       |
| p-button-icon-search-rounded-text-raised-success | PrimeNG Button with Search Icon, Rounded Text Raised Success style snippet |
| p-button-icon-search-rounded-text-success  | PrimeNG Button with Search Icon, Rounded Text Success style snippet  |
| p-button-icon-search-success               | PrimeNG Button with Search Icon, Success style snippet               |
| p-button-icon-times-danger                 | PrimeNG Button with Times Icon, Danger style snippet                 |
| p-button-icon-times-rounded-danger         | PrimeNG Button with Times Icon, Rounded Danger style snippet         |
| p-button-icon-times-rounded-outlined-danger| PrimeNG Button with Times Icon, Rounded Outlined Danger style snippet|
| p-button-icon-times-rounded-text-danger    | PrimeNG Button with Times Icon, Rounded Text Danger style snippet    |
| p-button-icon-times-rounded-text-raised-danger | PrimeNG Button with Times Icon, Rounded Text Raised Danger style snippet |
| p-button-icon-user-info                    | PrimeNG Button with User Icon, Info style snippet                    |
| p-button-icon-user-rounded-info            | PrimeNG Button with User Icon, Rounded Info style snippet            |
| p-button-icon-user-rounded-outlined-info   | PrimeNG Button with User Icon, Rounded Outlined Info style snippet   |
| p-button-icon-user-rounded-text-info       | PrimeNG Button with User Icon, Rounded Text Info style snippet       |
| p-button-icon-user-rounded-text-raised-info| PrimeNG Button with User Icon, Rounded Text Raised Info style snippet|
| p-button-info                              | PrimeNG Button with Info style snippet                               |
| p-button-info-outlined                     | PrimeNG Button with Info Outlined style snippet                      |
| p-button-info-raised                       | PrimeNG Button with Info Raised style snippet                        |
| p-button-info-rounded                      | PrimeNG Button with Info Rounded style snippet                       |
| p-button-info-text                         | PrimeNG Button with Info Text style snippet                          |
| p-button-info-text-raised                  | PrimeNG Button with Info Text Raised style snippet                   |
| p-button-large                             | PrimeNG Button in Large size snippet                                 |
| p-button-loading                           | PrimeNG Button with Loading state snippet                            |
| p-button-normal                            | PrimeNG Button in Normal size snippet                                |
| p-button-plain-text                        | PrimeNG Button with Plain Text style snippet                         |
| p-button-plain-text-raised                 | PrimeNG Button with Plain Text Raised style snippet                  |
| p-button-primary-outlined                  | PrimeNG Button with Primary Outlined style snippet                   |
| p-button-primary-raised                    | PrimeNG Button with Primary Raised style snippet                     |
| p-button-primary-rounded                   | PrimeNG Button with Primary Rounded style snippet                    |
| p-button-primary-text                      | PrimeNG Button with Primary Text style snippet                       |
| p-button-primary-text-raised               | PrimeNG Button with Primary Text Raised style snippet                |
| p-button-secondary                         | PrimeNG Button with Secondary style snippet                          |
| p-button-secondary-outlined                | PrimeNG Button with Secondary Outlined style snippet                 |
| p-button-secondary-raised                  | PrimeNG Button with Secondary Raised style snippet                   |
| p-button-secondary-rounded                 | PrimeNG Button with Secondary Rounded style snippet                  |
| p-button-secondary-text                    | PrimeNG Button with Secondary Text style snippet                     |
| p-button-secondary-text-raised             | PrimeNG Button with Secondary Text Raised style snippet              |
| p-button-small                             | PrimeNG Button in Small size snippet                                 |
| p-button-success                           | PrimeNG Button with Success style snippet                            |
| p-button-success-outlined                  | PrimeNG Button with Success Outlined style snippet                   |
| p-button-success-raised                    | PrimeNG Button with Success Raised style snippet                     |
| p-button-success-rounded                   | PrimeNG Button with Success Rounded style snippet                    |
| p-button-success-text                      | PrimeNG Button with Success Text style snippet                       |
| p-button-success-text-raised               | PrimeNG Button with Success Text Raised style snippet                |
| p-button-svg                               | PrimeNG Button with Custom SVG snippet                               |
| p-button-warn                              | PrimeNG Button with Warn style snippet                               |
| p-button-warn-outlined                     | PrimeNG Button with Warn Outlined style snippet                      |
| p-button-warn-raised                       | PrimeNG Button with Warn Raised style snippet                        |
| p-button-warn-rounded                      | PrimeNG Button with Warn Rounded style snippet                       |
| p-button-warn-text                         | PrimeNG Button with Warn Text style snippet                          |
| p-button-warn-text-raised                  | PrimeNG Button with Warn Text Raised style snippet                   |
| p-cascadeselect-import                     | Imports PrimeNG CascadeSelectModule in TypeScript                    |
| p-cascadeselect-basic                      | PrimeNG CascadeSelect component snippet                              |
| p-cascadeselect-disabled                   | PrimeNG CascadeSelect in Disabled state snippet                      |
| p-cascadeselect-filled                     | PrimeNG CascadeSelect with Filled style snippet                      |
| p-cascadeselect-float-label                | PrimeNG CascadeSelect with Float Label snippet                       |
| p-cascadeselect-ifta-label                 | PrimeNG CascadeSelect with Ifta Label snippet                        |
| p-cascadeselect-invalid                    | PrimeNG CascadeSelect in Invalid state snippet                       |
| p-cascadeselect-loading-state              | PrimeNG CascadeSelect with Loading State snippet                     |
| p-cascadeselect-reactive-forms             | PrimeNG CascadeSelect with Reactive Forms snippet                    |
| p-cascadeselect-sizes                      | PrimeNG CascadeSelect with different Sizes snippet                   |
| p-cascadeselect-template                   | PrimeNG CascadeSelect with Custom Template snippet                   |
| p-checkbox-import                          | Imports PrimeNG CheckboxModule in TypeScript                         |
| p-checkbox-basic                           | PrimeNG Checkbox component snippet                                   |
| p-checkbox-disabled                        | PrimeNG Checkbox in Disabled state snippet                           |
| p-checkbox-dynamic                         | PrimeNG Checkbox with Dynamic values snippet                         |
| p-checkbox-filled                          | PrimeNG Checkbox with Filled style snippet                           |
| p-checkbox-group                           | PrimeNG Checkbox Group component snippet                             |
| p-checkbox-indeterminate                   | PrimeNG Checkbox with Indeterminate state snippet                    |
| p-checkbox-invalid                         | PrimeNG Checkbox in Invalid state snippet                            |
| p-checkbox-large                           | PrimeNG Checkbox in Large size snippet                               |
| p-checkbox-normal                          | PrimeNG Checkbox in Normal size snippet                              |
| p-checkbox-reactive-form                   | PrimeNG Checkbox with Reactive Form snippet                          |
| p-checkbox-small                           | PrimeNG Checkbox in Small size snippet                               |
| p-colorpicker-import                       | Imports PrimeNG ColorPickerModule in TypeScript                      |
| p-colorpicker-basic                        | PrimeNG ColorPicker component snippet                                |
| p-colorpicker-disabled                     | PrimeNG ColorPicker in Disabled state snippet                        |
| p-colorpicker-hex                          | PrimeNG ColorPicker with HEX format snippet                          |
| p-colorpicker-hsb                          | PrimeNG ColorPicker with HSB format snippet                          |
| p-colorpicker-inline                       | PrimeNG ColorPicker in Inline mode snippet                           |
| p-colorpicker-reactive                     | PrimeNG ColorPicker with Reactive Forms snippet                      |
| p-colorpicker-rgb                          | PrimeNG ColorPicker with RGB format snippet                          |
| p-dataview-import                          | Imports PrimeNG DataViewModule in TypeScript                         |
| p-dataview-basic                           | PrimeNG DataView component snippet                                   |
| p-dataview-layout                          | PrimeNG DataView with Layout options snippet                         |
| p-dataview-loading                         | PrimeNG DataView with Loading state snippet                          |
| p-dataview-pagination                      | PrimeNG DataView with Pagination snippet                             |
| p-dataview-sorting                         | PrimeNG DataView with Sorting snippet                                |
| p-datepicker-import                        | Imports PrimeNG CalendarModule in TypeScript                         |
| p-datepicker-basic                         | PrimeNG DatePicker component snippet                                 |
| p-datepicker-button-bar                    | PrimeNG DatePicker with Button Bar snippet                           |
| p-datepicker-date-template                 | PrimeNG DatePicker with Date Template snippet                        |
| p-datepicker-disabled                      | PrimeNG DatePicker in Disabled state snippet                         |
| p-datepicker-filled                        | PrimeNG DatePicker with Filled style snippet                         |
| p-datepicker-float-label                   | PrimeNG DatePicker with Float Label snippet                          |
| p-datepicker-format                        | PrimeNG DatePicker with Custom Format snippet                        |
| p-datepicker-icon                          | PrimeNG DatePicker with Icon snippet                                 |
| p-datepicker-ifta-label                    | PrimeNG DatePicker with Ifta Label snippet                           |
| p-datepicker-inline                        | PrimeNG DatePicker in Inline mode snippet                            |
| p-datepicker-invalid                       | PrimeNG DatePicker in Invalid state snippet                          |
| p-datepicker-min-max                       | PrimeNG DatePicker with Min/Max range snippet                        |
| p-datepicker-month                         | PrimeNG DatePicker with Month Picker snippet                         |
| p-datepicker-multiple                      | PrimeNG DatePicker with Multiple selection snippet                   |
| p-datepicker-multiple-months               | PrimeNG DatePicker with Multiple Months snippet                      |
| p-datepicker-range                         | PrimeNG DatePicker with Range selection snippet                      |
| p-datepicker-reactive                      | PrimeNG DatePicker with Reactive Forms snippet                       |
| p-datepicker-sizes                         | PrimeNG DatePicker with different Sizes snippet                      |
| p-datepicker-time                          | PrimeNG DatePicker with Time selection snippet                       |
| p-datepicker-year                          | PrimeNG DatePicker with Year Picker snippet                          |
| p-editor-import                            | Imports PrimeNG EditorModule in TypeScript                           |
| p-editor-basic                             | PrimeNG Editor component snippet                                     |
| p-editor-quill-install                     | PrimeNG Editor Quill Installation snippet                            |
| p-editor-reactive                          | PrimeNG Editor with Reactive Forms snippet                           |
| p-editor-readonly                          | PrimeNG Editor in ReadOnly mode snippet                              |
| p-editor-template                          | PrimeNG Editor with Custom Template snippet                          |
| p-floatlabel-import                        | Imports PrimeNG FloatLabelModule in TypeScript                       |
| p-floatlabel-basic                         | PrimeNG FloatLabel component snippet                                 |
| p-floatlabel-in                            | PrimeNG FloatLabel with In style snippet                             |
| p-floatlabel-invalid                       | PrimeNG FloatLabel in Invalid state snippet                          |
| p-floatlabel-on                            | PrimeNG FloatLabel with On style snippet                             |
| p-floatlabel-over                          | PrimeNG FloatLabel with Over style snippet                           |
| p-floatlabel-variants                      | PrimeNG FloatLabel with Variants snippet                             |
| p-iconfield-import                         | Imports PrimeNG IconFieldModule in TypeScript                        |
| p-iconfield-basic                          | PrimeNG IconField component snippet                                  |
| p-iconfield-iftalabel                      | PrimeNG IconField with IftaLabel snippet                             |
| p-iconfield-sizes                          | PrimeNG IconField with different Sizes snippet                       |
| p-iconfield-template                       | PrimeNG IconField with Custom Template snippet                       |
| p-iftalabel-import                         | Imports PrimeNG IftaLabelModule in TypeScript                        |
| p-iftalabel-basic                          | PrimeNG IftaLabel component snippet                                  |
| p-iftalabel-invalid                        | PrimeNG IftaLabel in Invalid state snippet                           |
| p-inputgroup-import                        | Imports PrimeNG InputGroupModule in TypeScript                       |
| p-inputgroup-basic                         | PrimeNG InputGroup component snippet                                 |
| p-inputgroup-checkbox                      | PrimeNG InputGroup with Checkbox snippet                             |
| p-inputgroup-floatlabel                    | PrimeNG InputGroup with FloatLabel snippet                           |
| p-inputgroup-iftalabel                     | PrimeNG InputGroup with IftaLabel snippet                            |
| p-inputgroup-multiple                      | PrimeNG InputGroup with Multiple inputs snippet                      |
| p-inputgroup-price                         | PrimeNG InputGroup with Price format snippet                         |
| p-inputgroup-search                        | PrimeNG InputGroup with Search functionality snippet                 |
| p-inputmask-import                         | Imports PrimeNG InputMaskModule in TypeScript                        |
| p-inputmask-basic                          | PrimeNG InputMask component snippet                                  |
| p-inputmask-disabled                       | PrimeNG InputMask in Disabled state snippet                          |
| p-inputmask-filled                         | PrimeNG InputMask with Filled style snippet                          |
| p-inputmask-float-label                    | PrimeNG InputMask with Float Label snippet                           |
| p-inputmask-ifta-label                     | PrimeNG InputMask with Ifta Label snippet                            |
| p-inputmask-invalid                        | PrimeNG InputMask in Invalid state snippet                           |
| p-inputmask-mask                           | PrimeNG InputMask with Mask snippet                                  |
| p-inputmask-optional                       | PrimeNG InputMask with Optional values snippet                       |
| p-inputmask-reactive                       | PrimeNG InputMask with Reactive Forms snippet                        |
| p-inputmask-sizes                          | PrimeNG InputMask with different Sizes snippet                       |
| p-inputmask-slotchar                       | PrimeNG InputMask with SlotChar snippet                              |
| p-inputnumber-import                       | Imports PrimeNG InputNumberModule in TypeScript                      |
| p-inputnumber-buttons                      | PrimeNG InputNumber with Buttons snippet                             |
| p-inputnumber-currency                     | PrimeNG InputNumber with Currency format snippet                     |
| p-inputnumber-disabled                     | PrimeNG InputNumber in Disabled state snippet                        |
| p-inputnumber-filled                       | PrimeNG InputNumber with Filled style snippet                        |
| p-inputnumber-float-label                  | PrimeNG InputNumber with Float Label snippet                         |
| p-inputnumber-ifta-label                   | PrimeNG InputNumber with Ifta Label snippet                          |
| p-inputnumber-invalid                      | PrimeNG InputNumber in Invalid state snippet                         |
| p-inputnumber-locale                       | PrimeNG InputNumber with Locale settings snippet                     |
| p-inputnumber-numerals                     | PrimeNG InputNumber with Numerals snippet                            |
| p-inputnumber-prefix-suffix                | PrimeNG InputNumber with Prefix & Suffix snippet                     |
| p-inputnumber-reactive                     | PrimeNG InputNumber with Reactive Forms snippet                      |
| p-inputnumber-sizes                        | PrimeNG InputNumber with different Sizes snippet                     |
| p-inputnumber-vertical                     | PrimeNG InputNumber in Vertical mode snippet                         |
| p-inputotp-import                          | Imports PrimeNG InputOtpModule in TypeScript                         |
| p-inputotp-basic                           | PrimeNG InputOtp component snippet                                   |
| p-inputotp-integer-only                    | PrimeNG InputOtp with Integer Only snippet                           |
| p-inputotp-mask                            | PrimeNG InputOtp with Mask snippet                                   |
| p-inputotp-sample                          | PrimeNG InputOtp Sample snippet                                      |
| p-inputotp-sizes                           | PrimeNG InputOtp with different Sizes snippet                        |
| p-inputotp-template                        | PrimeNG InputOtp with Custom Template snippet                        |
| p-inputtext-import                         | Imports PrimeNG InputTextModule in TypeScript                        |
| p-inputtext-basic                          | PrimeNG InputText component snippet                                  |
| p-inputtext-disabled                       | PrimeNG InputText in Disabled state snippet                          |
| p-inputtext-filled                         | PrimeNG InputText with Filled style snippet                          |
| p-inputtext-float-label                    | PrimeNG InputText with Float Label snippet                           |
| p-inputtext-help-text                      | PrimeNG InputText with Help Text snippet                             |
| p-inputtext-ifta-label                     | PrimeNG InputText with Ifta Label snippet                            |
| p-inputtext-invalid                        | PrimeNG InputText in Invalid state snippet                           |
| p-inputtext-reactive                       | PrimeNG InputText with Reactive Forms snippet                        |
| p-inputtext-sizes                          | PrimeNG InputText with different Sizes snippet                       |
| p-keyfilter-import                         | Imports PrimeNG KeyFilterModule in TypeScript                        |
| p-keyfilter-alpha                          | PrimeNG KeyFilter with Alphabetic restriction snippet                |
| p-keyfilter-alphanum                       | PrimeNG KeyFilter with Alphanumeric restriction snippet              |
| p-keyfilter-hex                            | PrimeNG KeyFilter with Hex restriction snippet                       |
| p-keyfilter-int                            | PrimeNG KeyFilter with Integer restriction snippet                   |
| p-keyfilter-money                          | PrimeNG KeyFilter with Money restriction snippet                     |
| p-keyfilter-num                            | PrimeNG KeyFilter with Number restriction snippet                    |
| p-keyfilter-reactive                       | PrimeNG KeyFilter with Reactive Forms snippet                        |
| p-keyfilter-regex                          | PrimeNG KeyFilter with Regex restriction snippet                     |
| p-knob-import                              | Imports PrimeNG KnobModule in TypeScript                             |
| p-knob-basic                               | PrimeNG Knob component snippet                                       |
| p-knob-color                               | PrimeNG Knob with Color customization snippet                        |
| p-knob-disabled                            | PrimeNG Knob in Disabled state snippet                               |
| p-knob-min-max                             | PrimeNG Knob with Min/Max range snippet                              |
| p-knob-reactive                            | PrimeNG Knob with Reactive Forms snippet                             |
| p-knob-readonly                            | PrimeNG Knob in ReadOnly mode snippet                                |
| p-knob-size                                | PrimeNG Knob with Size customization snippet                         |
| p-knob-step                                | PrimeNG Knob with Step customization snippet                         |
| p-knob-stroke                              | PrimeNG Knob with Stroke customization snippet                       |
| p-knob-template                            | PrimeNG Knob with Custom Template snippet                            |
| p-listbox-import                           | Imports PrimeNG ListboxModule in TypeScript                          |
| p-listbox-basic                            | PrimeNG Listbox component snippet                                    |
| p-listbox-checkmark                        | PrimeNG Listbox with Checkmark snippet                               |
| p-listbox-disabled                         | PrimeNG Listbox in Disabled state snippet                            |
| p-listbox-filter                           | PrimeNG Listbox with Filter snippet                                  |
| p-listbox-group                            | PrimeNG Listbox with Group snippet                                   |
| p-listbox-invalid                          | PrimeNG Listbox in Invalid state snippet                             |
| p-listbox-multiple                         | PrimeNG Listbox with Multiple selection snippet                      |
| p-listbox-reactive                         | PrimeNG Listbox with Reactive Forms snippet                          |
| p-listbox-template                         | PrimeNG Listbox with Custom Template snippet                         |
| p-listbox-virtual-scroll                   | PrimeNG Listbox with Virtual Scroll snippet                          |
| p-multiSelect-import                       | Imports PrimeNG MultiSelectModule in TypeScript                      |
| p-multiselect-basic                        | PrimeNG MultiSelect component snippet                                |
| p-multiselect-chips                        | PrimeNG MultiSelect with Chips snippet                               |
| p-multiselect-disabled                     | PrimeNG MultiSelect in Disabled state snippet                        |
| p-multiselect-filled                       | PrimeNG MultiSelect with Filled style snippet                        |
| p-multiselect-filter                       | PrimeNG MultiSelect with Filter snippet                              |
| p-multiselect-float-label                  | PrimeNG MultiSelect with Float Label snippet                         |
| p-multiselect-group                        | PrimeNG MultiSelect with Group snippet                               |
| p-multiselect-ifta-label                   | PrimeNG MultiSelect with Ifta Label snippet                          |
| p-multiselect-invalid                      | PrimeNG MultiSelect in Invalid state snippet                         |
| p-multiselect-loading-state                | PrimeNG MultiSelect with Loading State snippet                       |
| p-multiselect-reactive-forms               | PrimeNG MultiSelect with Reactive Forms snippet                      |
| p-multiselect-sizes                        | PrimeNG MultiSelect with different Sizes snippet                     |
| p-multiselect-template                     | PrimeNG MultiSelect with Custom Template snippet                     |
| p-orderlist-import                         | Imports PrimeNG OrderListModule in TypeScript                        |
| p-orderlist-basic                          | PrimeNG OrderList component snippet                                  |
| p-orderlist-filter                         | PrimeNG OrderList with Filter snippet                                |
| p-orderlist-template                       | PrimeNG OrderList with Custom Template snippet                       |
| p-orgchart-import                          | Imports PrimeNG OrganizationChartModule in TypeScript                |
| p-orgchart-basic                           | PrimeNG OrganizationChart component snippet                          |
| p-orgchart-colored                         | PrimeNG OrganizationChart with Colored style snippet                 |
| p-orgchart-selection                       | PrimeNG OrganizationChart with Selection snippet                     |
| p-orgchart-template                        | PrimeNG OrganizationChart with Custom Template snippet               |
| p-paginator-import                         | Imports PrimeNG PaginatorModule in TypeScript                        |
| p-paginator-basic                          | PrimeNG Paginator component snippet                                  |
| p-paginator-current-page-report            | PrimeNG Paginator with Current Page Report snippet                   |
| p-paginator-template                       | PrimeNG Paginator with Custom Template snippet                       |
| p-password-import                          | Imports PrimeNG PasswordModule in TypeScript                         |
| p-password-basic                           | PrimeNG Password component snippet                                   |
| p-password-disabled                        | PrimeNG Password in Disabled state snippet                           |
| p-password-filled                          | PrimeNG Password with Filled style snippet                           |
| p-password-float-label                     | PrimeNG Password with Float Label snippet                            |
| p-password-ifta-label                      | PrimeNG Password with Ifta Label snippet                             |
| p-password-invalid                         | PrimeNG Password in Invalid state snippet                            |
| p-password-locale                          | PrimeNG Password with Locale settings snippet                        |
| p-password-meter                           | PrimeNG Password with Meter snippet                                  |
| p-password-reactive                        | PrimeNG Password with Reactive Forms snippet                         |
| p-password-sizes                           | PrimeNG Password with different Sizes snippet                        |
| p-password-template                        | PrimeNG Password with Custom Template snippet                        |
| p-password-toggle-mask                     | PrimeNG Password with Toggle Mask snippet                            |
| p-picklist-import                          | Imports PrimeNG PickListModule in TypeScript                         |
| p-picklist-basic                           | PrimeNG PickList component snippet                                   |
| p-picklist-filter                          | PrimeNG PickList with Filter snippet                                 |
| p-picklist-template                        | PrimeNG PickList with Custom Template snippet                        |
| p-radiobutton-import                       | Imports PrimeNG RadioButtonModule in TypeScript                      |
| p-radiobutton-disabled                     | PrimeNG RadioButton in Disabled state snippet                        |
| p-radiobutton-dynamic                      | PrimeNG RadioButton with Dynamic values snippet                      |
| p-radiobutton-filled                       | PrimeNG RadioButton with Filled style snippet                        |
| p-radiobutton-group                        | PrimeNG RadioButton Group snippet                                    |
| p-radiobutton-invalid                      | PrimeNG RadioButton in Invalid state snippet                         |
| p-radiobutton-reactive                     | PrimeNG RadioButton with Reactive Forms snippet                      |
| p-radiobutton-sizes                        | PrimeNG RadioButton with different Sizes snippet                     |
| p-rating-import                            | Imports PrimeNG RatingModule in TypeScript                           |
| p-rating-basic                             | PrimeNG Rating component snippet                                     |
| p-rating-disabled                          | PrimeNG Rating in Disabled state snippet                             |
| p-rating-reactive                          | PrimeNG Rating with Reactive Forms snippet                           |
| p-rating-readonly                          | PrimeNG Rating in ReadOnly mode snippet                              |
| p-rating-stars                             | PrimeNG Rating with Number of Stars snippet                          |
| p-rating-template                          | PrimeNG Rating with Custom Template snippet                          |
| p-select-import                            | Imports PrimeNG DropdownModule in TypeScript                         |
| p-select-basic                             | PrimeNG Select component snippet                                     |
| p-select-checkmark                         | PrimeNG Select with Checkmark snippet                                |
| p-select-clear                             | PrimeNG Select with Clear Icon snippet                               |
| p-select-disabled                          | PrimeNG Select in Disabled state snippet                             |
| p-select-editable                          | PrimeNG Select with Editable feature snippet                         |
| p-select-filled                            | PrimeNG Select with Filled style snippet                             |
| p-select-filter                            | PrimeNG Select with Filter snippet                                   |
| p-select-float-label                       | PrimeNG Select with Float Label snippet                              |
| p-select-group                             | PrimeNG Select with Group snippet                                    |
| p-select-ifta-label                        | PrimeNG Select with Ifta Label snippet                               |
| p-select-invalid                           | PrimeNG Select in Invalid state snippet                              |
| p-select-lazy-virtual-scroll               | PrimeNG Select with Lazy Virtual Scroll snippet                      |
| p-select-loading                           | PrimeNG Select with Loading State snippet                            |
| p-select-reactive                          | PrimeNG Select with Reactive Forms snippet                           |
| p-select-sizes                             | PrimeNG Select with different Sizes snippet                          |
| p-select-template                          | PrimeNG Select with Custom Template snippet                          |
| p-select-virtual-scroll                    | PrimeNG Select with Virtual Scroll snippet                           |
| p-selectbutton-import                      | Imports PrimeNG SelectButtonModule in TypeScript                     |
| p-selectbutton-basic                       | PrimeNG SelectButton component snippet                               |
| p-selectbutton-disabled                    | PrimeNG SelectButton in Disabled state snippet                       |
| p-selectbutton-invalid                     | PrimeNG SelectButton in Invalid state snippet                        |
| p-selectbutton-multiple                    | PrimeNG SelectButton with Multiple selection snippet                 |
| p-selectbutton-reactive                    | PrimeNG SelectButton with Reactive Forms snippet                     |
| p-selectbutton-sizes                       | PrimeNG SelectButton with different Sizes snippet                    |
| p-selectbutton-template                    | PrimeNG SelectButton with Custom Template snippet                    |
| p-slider-import                            | Imports PrimeNG SliderModule in TypeScript                           |
| p-slider-basic                             | PrimeNG Slider component snippet                                     |
| p-slider-filter                            | PrimeNG Slider with Filter snippet                                   |
| p-slider-input                             | PrimeNG Slider with Input snippet                                    |
| p-slider-range                             | PrimeNG Slider with Range snippet                                    |
| p-slider-reactive                          | PrimeNG Slider with Reactive Forms snippet                           |
| p-slider-step                              | PrimeNG Slider with Step customization snippet                       |
| p-slider-vertical                          | PrimeNG Slider in Vertical mode snippet                              |
| p-speeddial-import                         | Imports PrimeNG SpeedDialModule in TypeScript                        |
| p-speeddial-circle                         | PrimeNG SpeedDial in Circle layout snippet                           |
| p-speeddial-custom-button                  | PrimeNG SpeedDial with Custom Button snippet                         |
| p-speeddial-down                           | PrimeNG SpeedDial with Down direction snippet                        |
| p-speeddial-left                           | PrimeNG SpeedDial with Left direction snippet                        |
| p-speeddial-quartercircle-downright        | PrimeNG SpeedDial with Quarter-Circle Down-Right snippet             |
| p-speeddial-quartercircle-upleft           | PrimeNG SpeedDial with Quarter-Circle Up-Left snippet                |
| p-speeddial-right                          | PrimeNG SpeedDial with Right direction snippet                       |
| p-speeddial-semicircle-down                | PrimeNG SpeedDial with Semi-Circle Down snippet                      |
| p-speeddial-semicircle-up                  | PrimeNG SpeedDial with Semi-Circle Up snippet                        |
| p-speeddial-up                             | PrimeNG SpeedDial with Up direction snippet                          |
| p-splitbutton-import                       | Imports PrimeNG SplitButtonModule in TypeScript                      |
| p-splitbutton-basic                        | PrimeNG SplitButton component snippet                                |
| p-splitbutton-disabled                     | PrimeNG SplitButton in Disabled state snippet                        |
| p-splitbutton-icons                        | PrimeNG SplitButton with Icons snippet                               |
| p-splitbutton-nested                       | PrimeNG SplitButton with Nested items snippet                        |
| p-splitbutton-outlined                     | PrimeNG SplitButton with Outlined style snippet                      |
| p-splitbutton-raised                       | PrimeNG SplitButton with Raised style snippet                        |
| p-splitbutton-raised-text                  | PrimeNG SplitButton with Raised Text style snippet                   |
| p-splitbutton-rounded                      | PrimeNG SplitButton with Rounded style snippet                       |
| p-splitbutton-severity                     | PrimeNG SplitButton with Severity styles snippet                     |
| p-splitbutton-sizes                        | PrimeNG SplitButton with different Sizes snippet                     |
| p-splitbutton-template                     | PrimeNG SplitButton with Custom Template snippet                     |
| p-splitbutton-text                         | PrimeNG SplitButton with Text style snippet                          |
| p-table-import                             | Imports PrimeNG TableModule in TypeScript                            |
| p-table-basic                              | PrimeNG Table component snippet                                      |
| p-table-checkbox                           | PrimeNG Table with Checkbox Selection snippet                        |
| p-table-column-group                       | PrimeNG Table with Column Group snippet                              |
| p-table-column-selection                   | PrimeNG Table with Column Selection snippet                          |
| p-table-column-toggle                      | PrimeNG Table with Column Toggle snippet                             |
| p-table-conditional                        | PrimeNG Table with Conditional Style snippet                         |
| p-table-context-menu                       | PrimeNG Table with Context Menu snippet                              |
| p-table-dynamic                            | PrimeNG Table with Dynamic Columns snippet                           |
| p-table-edit-cell                          | PrimeNG Table with Edit Cell snippet                                 |
| p-table-edit-row                           | PrimeNG Table with Edit Row snippet                                  |
| p-table-events                             | PrimeNG Table with Events snippet                                    |
| p-table-export                             | PrimeNG Table with Export snippet                                    |
| p-table-filter-advanced                    | PrimeNG Table with Advanced Filter snippet                           |
| p-table-filter-basic                       | PrimeNG Table with Basic Filter snippet                              |
| p-table-flexible-scroll                    | PrimeNG Table with Flexible Scroll snippet                           |
| p-table-frozen-columns                     | PrimeNG Table with Frozen Columns snippet                            |
| p-table-frozen-rows                        | PrimeNG Table with Frozen Rows snippet                               |
| p-table-gridlines                          | PrimeNG Table with GridLines snippet                                 |
| p-table-horizontal-scroll                  | PrimeNG Table with Horizontal Scroll snippet                         |
| p-table-multiple-selection                 | PrimeNG Table with Multiple Selection snippet                        |
| p-table-multiple-sort                      | PrimeNG Table with Multiple Columns Sort snippet                     |
| p-table-pagination                         | PrimeNG Table with Pagination snippet                                |
| p-table-presort                            | PrimeNG Table with Presort snippet                                   |
| p-table-programmatic                       | PrimeNG Table with Programmatic control snippet                      |
| p-table-radiobutton                        | PrimeNG Table with RadioButton Selection snippet                     |
| p-table-removable-sort                     | PrimeNG Table with Removable Sort snippet                            |
| p-table-reorder                            | PrimeNG Table with Reorder snippet                                   |
| p-table-resize-expand                      | PrimeNG Table with Column Resize Expand snippet                      |
| p-table-resize-fit                         | PrimeNG Table with Column Resize Fit snippet                         |
| p-table-resize-scrollable                  | PrimeNG Table with Column Resize Scrollable snippet                  |
| p-table-row-expansion                      | PrimeNG Table with Row Expansion snippet                             |
| p-table-row-group-expandable               | PrimeNG Table with Row Group Expandable snippet                      |
| p-table-row-group-rowspan                  | PrimeNG Table with Row Group RowSpan snippet                         |
| p-table-row-group-subheader                | PrimeNG Table with Row Group Subheader snippet                       |
| p-table-row-selection-single               | PrimeNG Table with Row Selection Single snippet                      |
| p-table-sample-customers                   | PrimeNG Table with Sample Customers snippet                          |
| p-table-sample-products                    | PrimeNG Table with Sample Products snippet                           |
| p-table-scroll-vertical                    | PrimeNG Table with Vertical Scroll snippet                           |
| p-table-size                               | PrimeNG Table with Size customization snippet                        |
| p-table-sort-single                        | PrimeNG Table with Single Sort snippet                               |
| p-table-stateful                           | PrimeNG Table with Stateful behavior snippet                         |
| p-table-striped                            | PrimeNG Table with Striped Rows snippet                              |
| p-table-templated                          | PrimeNG Table with Templated content snippet                         |
| p-table-virtual-scroll-lazy                | PrimeNG Table with Virtual Scroll Lazy snippet                       |
| p-table-virtual-scroll-preload             | PrimeNG Table with Virtual Scroll Preload snippet                    |
| p-textarea-import                          | Imports PrimeNG InputTextareaModule in TypeScript                    |
| p-textarea-autoresize                      | PrimeNG Textarea with AutoResize snippet                             |
| p-textarea-basic                           | PrimeNG Textarea component snippet                                   |
| p-textarea-disabled                        | PrimeNG Textarea in Disabled state snippet                           |
| p-textarea-filled                          | PrimeNG Textarea with Filled style snippet                           |
| p-textarea-floatlabel                      | PrimeNG Textarea with FloatLabel snippet                             |
| p-textarea-iftalabel                       | PrimeNG Textarea with IftaLabel snippet                              |
| p-textarea-invalid                         | PrimeNG Textarea in Invalid state snippet                            |
| p-textarea-reactive                        | PrimeNG Textarea with Reactive Forms snippet                         |
| p-textarea-sizes                           | PrimeNG Textarea with different Sizes snippet                        |
| p-timeline-import                          | Imports PrimeNG TimelineModule in TypeScript                         |
| p-timeline-alignment                       | PrimeNG Timeline with Alignment customization snippet                |
| p-timeline-basic                           | PrimeNG Timeline component snippet                                   |
| p-timeline-horizontal                      | PrimeNG Timeline in Horizontal mode snippet                          |
| p-timeline-opposite                        | PrimeNG Timeline with Opposite content snippet                       |
| p-timeline-template                        | PrimeNG Timeline with Custom Template snippet                        |
| p-togglebutton-import                      | Imports PrimeNG ToggleButtonModule in TypeScript                     |
| p-toggleButton-basic                       | PrimeNG ToggleButton component snippet                               |
| p-toggleButton-disabled                    | PrimeNG ToggleButton in Disabled state snippet                       |
| p-toggleButton-icons                       | PrimeNG ToggleButton with Icons snippet                              |
| p-toggleButton-onChange                    | PrimeNG ToggleButton with OnChange Event snippet                     |
| p-toggleButton-styled                      | PrimeNG ToggleButton with Custom Styles snippet                      |
| p-tree-import                              | Imports PrimeNG TreeModule in TypeScript                             |
| p-tree-basic                               | PrimeNG Tree component snippet                                       |
| p-tree-checkbox                            | PrimeNG Tree with Checkbox Selection snippet                         |
| p-tree-context-menu                        | PrimeNG Tree with Context Menu snippet                               |
| p-tree-controlled                          | PrimeNG Tree with Controlled behavior snippet                        |
| p-tree-dragdrop                            | PrimeNG Tree with DragDrop snippet                                   |
| p-tree-events                              | PrimeNG Tree with Events snippet                                     |
| p-tree-filter                              | PrimeNG Tree with Filter snippet                                     |
| p-tree-lazy                                | PrimeNG Tree with Lazy Loading snippet                               |
| p-tree-multi-select                        | PrimeNG Tree with Multiple Selection snippet                         |
| p-tree-single-select                       | PrimeNG Tree with Single Selection snippet                           |
| p-tree-template                            | PrimeNG Tree with Custom Template snippet                            |
| p-tree-virtual-scroll                      | PrimeNG Tree with Virtual Scroll snippet                             |
| p-treetable-import                         | Imports PrimeNG TreeTableModule in TypeScript                        |
| p-treetable-basic                          | PrimeNG TreeTable component snippet                                  |
| p-treetable-column-group                   | PrimeNG TreeTable with Column Group snippet                          |
| p-treetable-column-toggle                  | PrimeNG TreeTable with Column Toggle snippet                         |
| p-treetable-conditional-style              | PrimeNG TreeTable with Conditional Style snippet                     |
| p-treetable-context-menu                   | PrimeNG TreeTable with Context Menu snippet                          |
| p-treetable-controlled                     | PrimeNG TreeTable with Controlled behavior snippet                   |
| p-treetable-dynamic                        | PrimeNG TreeTable with Dynamic Columns snippet                       |
| p-treetable-events                         | PrimeNG TreeTable with Events snippet                                |
| p-treetable-filter                         | PrimeNG TreeTable with Filter snippet                                |
| p-treetable-frozen-columns                 | PrimeNG TreeTable with Frozen Columns snippet                        |
| p-treetable-gridlines                      | PrimeNG TreeTable with Grid Lines snippet                            |
| p-treetable-lazy-load                      | PrimeNG TreeTable with Lazy Load snippet                             |
| p-treetable-paginator-basic                | PrimeNG TreeTable with Paginator Basic snippet                       |
| p-treetable-paginator-locale               | PrimeNG TreeTable with Paginator Locale snippet                      |
| p-treetable-paginator-template             | PrimeNG TreeTable with Paginator Template snippet                    |
| p-treetable-reorder                        | PrimeNG TreeTable with Reorder snippet                               |
| p-treetable-resize-expand                  | PrimeNG TreeTable with Column Resize Expand snippet                  |
| p-treetable-resize-fit                     | PrimeNG TreeTable with Column Resize Fit snippet                     |
| p-treetable-resize-scrollable              | PrimeNG TreeTable with Column Resize Scrollable snippet              |
| p-treetable-scroll-flexible                | PrimeNG TreeTable with Scroll Flexible snippet                       |
| p-treetable-scroll-horizontal              | PrimeNG TreeTable with Scroll Horizontal snippet                     |
| p-treetable-scroll-vertical                | PrimeNG TreeTable with Scroll Vertical snippet                       |
| p-treetable-selection-checkbox             | PrimeNG TreeTable with Selection Checkbox snippet                    |
| p-treetable-selection-multiple             | PrimeNG TreeTable with Selection Multiple snippet                    |
| p-treetable-selection-single               | PrimeNG TreeTable with Selection Single snippet                      |
| p-treetable-size                           | PrimeNG TreeTable with Size customization snippet                    |
| p-treetable-sort-multiple                  | PrimeNG TreeTable with Sort Multiple snippet                         |
| p-treetable-sort-single                    | PrimeNG TreeTable with Sort Single snippet                           |
| p-treetable-template                       | PrimeNG TreeTable with Custom Template snippet                       |
| p-virtualscroller-import                   | Imports PrimeNG ScrollerModule in TypeScript                         |
| p-virtualscroller-basic                    | PrimeNG Scroller component snippet                                   |
| p-virtualscroller-delay                    | PrimeNG Scroller with Delay snippet                                  |
| p-virtualscroller-grid                     | PrimeNG Scroller with Grid layout snippet                            |
| p-virtualscroller-horizontal               | PrimeNG Scroller with Horizontal layout snippet                      |
| p-virtualscroller-lazy                     | PrimeNG Scroller with Lazy loading snippet                           |
| p-virtualscroller-loading                  | PrimeNG Scroller with Loading state snippet                          |
| p-virtualscroller-programmatic             | PrimeNG Scroller with Programmatic control snippet                   |
| p-virtualscroller-template                 | PrimeNG Scroller with Custom Template snippet                        |