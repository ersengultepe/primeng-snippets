# PrimeNG Quickly for VS Code

**Created for PrimeNG Quickly release**

This extension for Visual Studio Code includes a lot of primeNG elements that allow you to quickly add snippets in Typescript and HTML files if you install PrimeNG in your Angular applications.
Currently snippets for form elements are available, but will be updated frequently for other primeNG elements. 
Stay tuned !!!

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

# Using npm
```sh
npm install primeng @primeng/themes primeicons primeflex
```

# Using yarn

```sh
yarn add primeng @primeng/themes primeicons primeflex
```
# Using pnpm

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

### Available PrimeNG Components in Snippets

AutoComplete, CascadeSelect, Checkbox, ColorPicker, DatePicker, Editor, FloatLabel, IconField, InputGroup, InputMask, InputNumber, InputOTP, InputText, KeyFilter, Knob, ListBox, MultiSelect, Password, RadioButton, Rating, Select, SelectButton, Slider, TextArea, ToggleButton, ToggleSwitch, TreeSelect, Button, SpeedDial.

## Available PrimeNG Components in Snippets

| Snippet                                    | Purpose                                                              |
|--------------------------------------------|----------------------------------------------------------------------|
| p-autocomplete-import                      | Imports PrimeNG AutoCompleteModule in TypeScript                     |
| p-autocomplete-basic                       | PrimeNG AutoComplete component snippet                               |
| p-cascadeselect-import                     | Imports PrimeNG CascadeSelectModule in TypeScript                    |
| p-cascadeselect-basic                      | PrimeNG CascadeSelect component snippet                              |
| p-checkbox-import                          | Imports PrimeNG CheckboxModule in TypeScript                         |
| p-checkbox-basic                           | PrimeNG Checkbox component snippet                                   |
| p-colorpicker-import                       | Imports PrimeNG ColorPickerModule in TypeScript                      |
| p-colorpicker-basic                        | PrimeNG ColorPicker component snippet                                |
| p-datepicker-import                        | Imports PrimeNG DatePickerModule in TypeScript                       |
| p-datepicker-basic                         | PrimeNG DatePicker component snippet                                 |
| p-editor-import                            | Imports PrimeNG EditorModule in TypeScript                           |
| p-editor-basic                             | PrimeNG Editor component snippet                                     |
| p-floatlabel-import                        | Imports PrimeNG FloatLabelModule in TypeScript                       |
| p-floatlabel-basic                         | PrimeNG FloatLabel component snippet                                 |
| p-iconfield-import                         | Imports PrimeNG IconFieldModule in TypeScript                        |
| p-iconfield-basic                          | PrimeNG IconField component snippet                                  |
| p-inputgroup-import                        | Imports PrimeNG InputGroupModule in TypeScript                       |
| p-inputgroup-basic                         | PrimeNG InputGroup component snippet                                 |
| p-inputmask-import                         | Imports PrimeNG InputMaskModule in TypeScript                        |
| p-inputmask-basic                          | PrimeNG InputMask component snippet                                  |
| p-inputnumber-import                       | Imports PrimeNG InputNumberModule in TypeScript                      |
| p-inputnumber-basic                        | PrimeNG InputNumber component snippet                                |
| p-inputotp-import                          | Imports PrimeNG InputOTPModule in TypeScript                         |
| p-inputotp-basic                           | PrimeNG InputOTP component snippet                                   |
| p-inputtext-import                         | Imports PrimeNG InputTextModule in TypeScript                        |
| p-inputtext-basic                          | PrimeNG InputText component snippet                                  |
| p-keyfilter-import                         | Imports PrimeNG KeyFilterModule in TypeScript                        |
| p-keyfilter-basic                          | PrimeNG KeyFilter component snippet                                  |
| p-knob-import                              | Imports PrimeNG KnobModule in TypeScript                             |
| p-knob-basic                               | PrimeNG Knob component snippet                                       |
| p-listbox-import                           | Imports PrimeNG ListBoxModule in TypeScript                          |
| p-listbox-basic                            | PrimeNG ListBox component snippet                                    |
| p-multiselect-import                       | Imports PrimeNG MultiSelectModule in TypeScript                      |
| p-multiselect-basic                        | PrimeNG MultiSelect component snippet                                |
| p-password-import                          | Imports PrimeNG PasswordModule in TypeScript                         |
| p-password-basic                           | PrimeNG Password component snippet                                   |
| p-radiobutton-import                       | Imports PrimeNG RadioButtonModule in TypeScript                      |
| p-radiobutton-basic                        | PrimeNG RadioButton component snippet                                |
| p-rating-import                            | Imports PrimeNG RatingModule in TypeScript                           |
| p-rating-basic                             | PrimeNG Rating component snippet                                     |
| p-select-import                            | Imports PrimeNG SelectModule in TypeScript                           |
| p-select-basic                             | PrimeNG Select component snippet                                     |
| p-selectbutton-import                      | Imports PrimeNG SelectButtonModule in TypeScript                     |
| p-selectbutton-basic                       | PrimeNG SelectButton component snippet                               |
| p-slider-import                            | Imports PrimeNG SliderModule in TypeScript                           |
| p-slider-basic                             | PrimeNG Slider component snippet                                     |
| p-textarea-import                          | Imports PrimeNG TextAreaModule in TypeScript                         |
| p-textarea-basic                           | PrimeNG TextArea component snippet                                   |
| p-togglebutton-import                      | Imports PrimeNG ToggleButtonModule in TypeScript                     |
| p-togglebutton-basic                       | PrimeNG ToggleButton component snippet                               |
| p-toggleswitch-import                      | Imports PrimeNG ToggleSwitchModule in TypeScript                     |
| p-toggleswitch-basic                       | PrimeNG ToggleSwitch component snippet                               |
| p-treeselect-import                        | Imports PrimeNG TreeSelectModule in TypeScript                       |
| p-treeselect-basic                         | PrimeNG TreeSelect component snippet                                 |
| p-button-import                            | Imports PrimeNG ButtonModule in TypeScript                           |
| p-button-basic                             | PrimeNG Button component snippet                                     |
| p-speeddial-import                         | Imports PrimeNG SpeedDialModule in TypeScript                        |
| p-speeddial-basic                          | PrimeNG SpeedDial component snippet                                  |


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

##

Plugin logo created by Canva

- [Canva - Free Online AI Image Generator](https://www.canva.com/ai-image-generator/)

![Logo](images/logo.png)

