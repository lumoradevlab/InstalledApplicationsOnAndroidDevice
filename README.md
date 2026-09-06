# InstalledApplicationsOnAndroidDevice

An Android app that reads the **list of applications installed on the device** through
`PackageManager` and shows them as a launcher-style icon grid.

## What it does

- Queries `PackageManager` for installed packages, keeping each app's icon (`Drawable`) and label.
- Renders them in a 4-column `GridLayoutManager` inside a RecyclerView.
- Pages the grid with a `ViewPager`, where each page is an `AppListFragment` given a start and end
  index into the shared list — so the pager holds pages of apps rather than one long scroll.

`Kotlin` · `PackageManager` · `RecyclerView` · `ViewPager`
