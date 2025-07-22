# onPlatformMaui
Issue with OnPlatform for AOT trimming for grids

With the OnPlatform commented in

```
 <ColumnDefinition>
      <ColumnDefinition.Width>
          <OnPlatform x:TypeArguments="GridLength" Default="220">
              <On Platform="Android" Value="250"></On>
          </OnPlatform>
      </ColumnDefinition.Width>
  </ColumnDefinition>
```

The app crashes

With it commented out no crash or using the platformextension

```<ColumnDefinition Width="{OnPlatform iOS='245', Android='250', WinUI='255'}" />```

Inline Onplatforms work fine

![OnPlatform commented in](https://github.com/user-attachments/assets/5767ffdc-608f-499e-b2fc-4df9bcd7e1bc)

OnPlatform commented out
![OnPlatform commented in](https://github.com/user-attachments/assets/f6c611b5-5387-44de-b97c-8314b8a9800e)

