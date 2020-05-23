# Forge UI Snippets

This extension for Visual Studio Code adds snippets for [Forge UI](https://developer.atlassian.com/platform/forge/ui-components/). Supports .jsx file extension.

## Usage

Type part of a snippet, press enter, and the snippet unfolds.

| Shortcut Identifier | Component                | Code                                      |
| ------------------: | ------------------------ | ----------------------------------------- |
|             `fbtn→` | Button component         | [Button code](#ButtonCode)                |
|            `fbtns→` | ButtonSet component      | [ButtonSet code](#ButtonSetCode)          |
|             `ftxt→` | Text component           | [Text code](#TextCode)                    |
|            `ftxts→` | Text strong component    | [Text strong code](#TextStrongCode)       |
|            `ftxte→` | Text emphasis component  | [Text emphasis code](#TextEmphasisCode)   |
|         `ftxtstri→` | Text strike component    | [Text strike code](#TextStrikeCode)       |
|            `ftxtl→` | Text link component      | [Text link code](#TextLinkCode)           |
|            `ftxtc→` | Code component           | [Code](#Code)                             |
|           `ftxtul→` | Unordered list component | [Unordered list code](#UnorderedListCode) |
|           `ftxtol→` | Ordered list component   | [Ordered list code](#OrderedListCode)     |
|           `ftxtlo→` | Lozenge component        | [Lozenge code](#LozengeCode)              |
|           `ftxtdl→` | DateLozenge component    | [DateLozenge code](#DateLozengeCode)      |
|          `ffrgmnt→` | Fragment component       | [Fragment code](#FragmentCode)            |
|             `fimg→` | Image component          | [Image code](#ImageCode)                  |
|            `fmodd→` | ModalDialog component    | [ModalDialog code](#ModalDialogCode)      |
|            `ftabl→` | Table component          | [Table code](#TableCode)                  |
|            `fform→` | Form component           | [Form code](#FormCode)                    |

Alternatively, press Ctrl+Space to activate snippets from within the editor.

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

## TextLinkCode

**Shortcut**: _ftxtl→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>[It's a link to Forge](https://www.atlassian.com/forge)</Text>
```

## Code

**Shortcut**: _ftxtc→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text>{`<Text>sample text</Text>`}</Text>
```

## UnorderedListCode

**Shortcut**: _ftxtul→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text> - Item 1 </Text>
<Text> - Item 2 </Text>
<Text> - Item 3 </Text>
<Text> - Item 4 </Text>
```

## OrderedListCode

**Shortcut**: _ftxtol→_
[Text component](https://developer.atlassian.com/platform/forge/ui-components/text/)

```jsx
<Text> 1. Item 1 </Text>
<Text> 2. Item 2 </Text>
<Text> 3. Item 3 </Text>
<Text> 4. Item 4 </Text>
```

## LozengeCode

**Shortcut**: _ftxtlo→_
[Lozenge component](https://developer.atlassian.com/platform/forge/ui-components/text/#lozenge)

```jsx
<Text>
  You have 4 tickets: <Lozenge text="In progress" appearance="inprogress" />
</Text>
```

## DateLozenge

**Shortcut**: _ftxtdl→_
[DateLozenge component](https://developer.atlassian.com/platform/forge/ui-components/text/#lozenge)

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
