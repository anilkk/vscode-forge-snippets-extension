# Forge UI Snippets

This extension for Visual Studio Code adds snippets for [Forge UI](https://developer.atlassian.com/platform/forge/ui-components/). Supports .jsx file extension.

## Usage

Type part of a snippet, press enter, and the snippet unfolds.

| Shortcut Identifier | Component                    | Code                                               |
| ------------------: | ---------------------------- | -------------------------------------------------- |
|             `fbtn→` | Button component             | [Button](#ButtonCode)                              |
|            `fbtns→` | ButtonSet component          | [ButtonSet](#ButtonSetCode)                        |
|             `ftxt→` | Text component               | [Text](#TextCode)                                  |
|            `ftxts→` | Text strong component        | [Text strong](#TextStrongCode)                     |
|            `ftxte→` | Text emphasis component      | [Text emphasis](#TextEmphasisCode)                 |
|         `ftxtstri→` | Text strike component        | [Text strike](#TextStrikeCode)                     |
|            `flink→` | Link component               | [Link](#LinkCode)                                  |
|            `fcode→` | Code component               | [Code](#Code)                                      |
|           `flistu→` | Unordered list component     | [Unordered list](#UnorderedListCode)               |
|           `flisto→` | Ordered list component       | [Ordered list](#OrderedListCode)                   |
|             `floz→` | Lozenge component            | [Lozenge](#LozengeCode)                            |
|            `fdate→` | DateLozenge component        | [DateLozenge](#DateLozengeCode)                    |
|          `ffrgmnt→` | Fragment component           | [Fragment](#FragmentCode)                          |
|             `fimg→` | Image component              | [Image](#ImageCode)                                |
|            `fmodd→` | ModalDialog component        | [ModalDialog](#ModalDialogCode)                    |
|            `ftabl→` | Table component              | [Table](#TableCode)                                |
|            `fform→` | Form component               | [Form](#FormCode)                                  |
|          `fformtf→` | Form TextField component     | [Form TextField](#FormTextFieldCode)               |
|          `fformta→` | Form TextArea component      | [Form TextArea](#FormTextAreaCode)                 |
|           `fforms→` | Form Select component        | [Form Select](#FormSelectCode)                     |
|          `fformrg→` | Form RadioGroup component    | [Form RadioGroup](#FormRadioGroupCode)             |
|          `fformdp→` | Form DatePicker component    | [Form DatePicker](#FormDatePickerCode)             |
|          `fformcg→` | Form CheckboxGroup component | [Form CheckboxGroup](#FormCheckboxGroupCode)       |
|          `fformup→` | Form UserPicker component    | [Form UserPicker](#FormUserPickerCode)             |
|      `fconfigform→` | ConfigForm component         | [ConfigForm CheckboxGroup](#FormCheckboxGroupCode) |
|          `favatar→` | Avatar component             | [Avatar](#AvatarCode)                              |
|         `favatars→` | AvatarStack component        | [AvatarStack](#FormUsAvatarStackCode)              |

Alternatively, press Ctrl+Space to activate snippets from within the editor.

## Not supported components

Currently, the following components shortcuts are not available. Most of the time, following code components code, is generated while you create the specific type of Forge app.

1. [ContentAction](https://developer.atlassian.com/platform/forge/ui-components/content-action/)
2. [ContextMenu](https://developer.atlassian.com/platform/forge/ui-components/context-menu/)
3. [InlineDialog](https://developer.atlassian.com/platform/forge/ui-components/inline-dialog/)
4. [IssueGlance](https://developer.atlassian.com/platform/forge/ui-components/issue-glance/)
5. [IssuePanel](https://developer.atlassian.com/platform/forge/ui-components/issue-panel/)
6. [Macro](https://developer.atlassian.com/platform/forge/ui-components/macro/)

## Forge UI hooks

Coming soon...

## Installation

1. Install Visual Studio Code 1.45.1 or higher
2. Launch VS Code
3. From the command palette Ctrl-Shift-P (Windows, Linux) or Cmd-Shift-P (macOS)
4. Select Install Extension
5. Choose the extension Forge Snippets
6. Reload VS Code

## ButtonCode

**Shortcut**: _fbtn→_
[Button component](https://developer.atlassian.com/platform/forge/ui-components/button/)

```jsx
<Button
  text="button text"
  onClick={() => console.log('perform button click action')}
/>
```

## ButtonSetCode

**Shortcut**: _fbtns→_
[ButtonSet component](https://developer.atlassian.com/platform/forge/ui-components/button-set/)

```jsx
<ButtonSet>
  <Button
    text="button text 1"
    onClick={() => console.log('perform button 1 click action')}
  />
  <Button
    ext="button text 2"
    onClick={() => console.log('perform button 2 click action')}
  />
</ButtonSet>
```

## TextCode

**Shortcut**: _ftxt→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>sample text</Text>
```

## TextStrongCode

**Shortcut**: _ftxts→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>**It's a strong text**</Text>
```

## TextEmphasisCode

**Shortcut**: _ftxte→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>*It's a emphasis text*</Text>
```

## TextStrikeCode

**Shortcut**: _ftxtstri→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>~~strike~~</Text>
```

## LinkCode

**Shortcut**: _flink→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>[It's a link to Forge](https://www.atlassian.com/forge)</Text>
```

## Code

**Shortcut**: _fcode→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>{`<Text>sample text</Text>`}</Text>
```

## UnorderedListCode

**Shortcut**: _flistu→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text> - Item 1 </Text>
<Text> - Item 2 </Text>
<Text> - Item 3 </Text>
<Text> - Item 4 </Text>
```

## OrderedListCode

**Shortcut**: _flisto→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text> 1. Item 1 </Text>
<Text> 2. Item 2 </Text>
<Text> 3. Item 3 </Text>
<Text> 4. Item 4 </Text>
```

## LozengeCode

**Shortcut**: _floz→_
[Lozenge component](https://developer.atlassian.com/platform/forge/ui-components/text/#lozenge)

```jsx
<Text>
  You have 4 tickets: <Lozenge text="In progress" appearance="inprogress" />
</Text>
```

## DateLozenge

**Shortcut**: _fdate→_
[DateLozenge component](https://developer.atlassian.com/platform/forge/ui-components/text/#datelozenge)

```jsx
<Text>
  <DateLozenge value={new Date('07-29-1988').getTime()} />
</Text>
```

## FragmentCode

**Shortcut**: _ffrgmnt→_
[Fragment component](https://developer.atlassian.com/platform/forge/ui-components/fragment/)

```jsx
<Fragment>
  <Text content="Hello world!" />
  <Button text="Do something" onClick={onClick} />
</Fragment>
```

## ImageCode

**Shortcut**: _fimg→_
[Image component](https://developer.atlassian.com/platform/forge/ui-components/image/)

````jsx
<Image
  src="https://media.giphy.com/media/jUwpNzg9IcyrK/source.gif"
  alt="homer"
/>

## ModalDialog

**Shortcut**: _fmodd→_
[ModalDialog component](https://developer.atlassian.com/platform/forge/ui-components/modal-dialog/)

```jsx
<Button text="Show modal" onClick={() => setOpen(true)} />
{isOpen && (
<ModalDialog header=\"My modal dialog\" onClose={() => setOpen(false)}>
<Text>Hello there!</Text>
</ModalDialog>"
)}
````

## TableCode

**Shortcut**: _ftabl→_
[Table component](https://developer.atlassian.com/platform/forge/ui-components/table/)

```jsx
<Table>
  <Head>
    <Cell>
      <Text content="Header Column 1=" />
    </Cell>
    <Cell>
      <Text content="Header Column 2=" />
    </Cell>
  </Head>
  <Row>
    <Cell>
      <Text content="Row 1 Column 1=" />
    </Cell>
    <Cell>
      <Text content="Row 1 Column 2=" />
    </Cell>
  </Row>
</Table>
```

## Form

**Shortcut**: _fform→_
[Form component](https://developer.atlassian.com/platform/forge/ui-components/form/)

```jsx
<Form onSubmit={setSubmitted}>
  <TextField name="username" label="Username" />
  <CheckboxGroup name="products" legend="Products">
    <Checkbox defaultChecked value="jira" label="Jira" />
    <Checkbox value="confluence" label="Confluence" />
  </CheckboxGroup>
</Form>
```

## FormTextFieldCode

**Shortcut**: _fformtf→_
[Form TextField component](https://developer.atlassian.com/platform/forge/ui-components/form/#textfield)

```jsx
<TextField label="Name" name="name" />
```

## FormTextAreaCode

**Shortcut**: _fformta→_
[Form TextArea component](https://developer.atlassian.com/platform/forge/ui-components/form/#textarea)

```jsx
<TextArea label="Message" name="message" />
```

## FormSelectCode

**Shortcut**: _fforms→_
[Form Select component](https://developer.atlassian.com/platform/forge/ui-components/form/#select)

```jsx
<Select label="With a defaultSelected" name="milestone">
  <Option defaultSelected label="Milestone 1" value="one" />
  <Option label="Milestone 2" value="two" />
  <Option label="Milestone 3" value="three" />
</Select>
```

## FormRadioGroupCode

**Shortcut**: _fformrg→_
[Form RadioGroup component](https://developer.atlassian.com/platform/forge/ui-components/form/#radiogroup)

```jsx
<RadioGroup name="flavor" label="Pick a flavor">
  <Radio defaultChecked label="Strawberry" value="strawberry" />
  <Radio label="Cinnamon" value="cinnamon" />
  <Radio label="Chocolate" value="chocolate" />
</RadioGroup>
```

## FormDatePickerCode

**Shortcut**: _fformdp→_
[Form DatePicker component](https://developer.atlassian.com/platform/forge/ui-components/form/#datepicker)

```jsx
<DatePicker name="date" label="Appointment Date" />
```

## FormCheckboxGroupCode

**Shortcut**: _fformcg→_
[Form CheckboxGroup component](https://developer.atlassian.com/platform/forge/ui-components/form/#checkboxgroup)

```jsx
<CheckboxGroup legend="Products" name="products">
  <Checkbox value="jira" label="Jira" />
  <Checkbox value="confluence" label="Confluence" />
</CheckboxGroup>
```

## FormUserPickerCode

**Shortcut**: _fformup→_
[Form UserPicker component](https://developer.atlassian.com/platform/forge/ui-components/form/#userpicker)

```jsx
<UserPicker label="User" name="user" />
```

## ConfigForm

**Shortcut**: _fconfigform→_
[ConfigForm component](https://developer.atlassian.com/platform/forge/ui-components/form/#configform)

```jsx
const Config = () => {
  return (
    <ConfigForm>
      <TextField name="name" label="Pet name" />
      <TextField name="age" label="Pet age" />
    </ConfigForm>
  );
};
```

## AvatarCode

**Shortcut**: _favatar→_
[Avatar component](https://developer.atlassian.com/platform/forge/ui-components/avatar)

```jsx
<Avatar accountId="5a1234bc8d12345e3f1g11hi" />
```

## AvatarStackCode

**Shortcut**: _favatars→_
[AvatarStack component](https://developer.atlassian.com/platform/forge/ui-components/avatar-stack)

```jsx
<AvatarStack>
  <Avatar accountId="5a1234bc8d12345e3f1g11hi" />
  <Avatar accountId="2a98a42dbc7ab42e12ee360d" />
  <Avatar accountId="5d8732lq8jg85a0e3f1g90as" />
  <Avatar accountId="2h98a10dbl5ab93e62hja23z" />
  <Avatar accountId="7b20f0bc2d05325e3f1g43ty" />
  <Avatar accountId="2p72s42dbc7ab42e90gf252d" />
  <Avatar accountId="2l01x78mf4pqw42e84fg40ad" />
</AvatarStack>
```
