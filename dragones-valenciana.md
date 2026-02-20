This code defines a sealed interface `CloseTabsDialogType` that represents three possible “close tabs” actions in a dialog:

```kotlin
private sealed interface CloseTabsDialogType {
    object CloseAll : CloseTabsDialogType
    object CloseAllIncognito : CloseTabsDialogType
    object CloseSelected : CloseTabsDialogType
}
```

It has three implementations: `CloseAll` for closing all tabs, `CloseAllIncognito` for closing all incognito tabs, and `CloseSelected` for closing only selected tabs. [chrome](chrome://newtab/)