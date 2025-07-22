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

With it commented out or using the platformextension there is no crash

```<ColumnDefinition Width="{OnPlatform iOS='245', Android='250', WinUI='255'}" />```

With the OnPlatform commented in we get this crash

![OnPlatform commented in](https://github.com/user-attachments/assets/5767ffdc-608f-499e-b2fc-4df9bcd7e1bc)

OnPlatform commented out, although the platform extension version is still there no crash
![OnPlatform commented in](https://github.com/user-attachments/assets/f6c611b5-5387-44de-b97c-8314b8a9800e)

