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

With it commented out no crash

Inline Onplatforms work fine

![Crash](OnPlatform commented in.jpg)

![Working](OnPlatform commented out.jpg?raw=true)
