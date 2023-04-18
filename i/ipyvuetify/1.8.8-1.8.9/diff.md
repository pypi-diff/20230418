# Comparing `tmp/ipyvuetify-1.8.8.tar.gz` & `tmp/ipyvuetify-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvuetify-1.8.8.tar", last modified: Tue Apr  4 16:08:42 2023, max compression
+gzip compressed data, was "ipyvuetify-1.8.9.tar", last modified: Tue Apr  4 19:21:01 2023, max compression
```

## Comparing `ipyvuetify-1.8.8.tar` & `ipyvuetify-1.8.9.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.556258 ipyvuetify-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 16:08:42.556258 ipyvuetify-1.8.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5680 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.512257 ipyvuetify-1.8.8/ipyvuetify/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/Html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/Themes.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/VuetifyTemplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.512257 ipyvuetify-1.8.8/ipyvuetify/extra/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/extra/file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/ipyvuetify/extra/file_input.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.532258 ipyvuetify-1.8.8/ipyvuetify/generated/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/App.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/AppBar.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/AppBarNavIcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Avatar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Badge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/BottomNavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/BottomSheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Breadcrumbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/BreadcrumbsDivider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/BreadcrumbsItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Btn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/BtnToggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CalendarDaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CalendarMonthly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CalendarWeekly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Card.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CardActions.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CardSubtitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CardText.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CardTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Carousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CarouselItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CarouselReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/CarouselTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ChipGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ColorPicker.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ColorPickerCanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ColorPickerSwatches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Content.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DataFooter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DataIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DataTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DataTableHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerDateTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerMonthTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerYears.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DialogBottomTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/DialogTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Divider.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/EditDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpandTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpandXTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanelContent.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanelHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanels.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/FabTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/FadeTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/FileInput.py
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Footer.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Form.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Hover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Img.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Item.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ItemGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Label.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/List.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemAction.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemActionText.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemAvatar.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemContent.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemIcon.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemSubtitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ListItemTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/MenuTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/NavigationDrawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/OverflowBtn.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Parallax.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Picker.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ProgressCircular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ProgressLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/RadioGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/RangeSlider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Row.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ScaleTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ScrollXReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ScrollXTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ScrollYReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ScrollYTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SimpleCheckbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SimpleTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SkeletonLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideXReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideXTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideYReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SlideYTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Snackbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Spacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SpeedDial.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/StepperContent.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/StepperHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/StepperItems.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/StepperStep.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Subheader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/SystemBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Tab.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TabItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TabReverseTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TabTransition.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TableOverflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TabsItems.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TabsSlider.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TextField.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Textarea.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ThemeProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TimePicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TimePickerClock.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TimePickerTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TimelineItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ToolbarItems.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/ToolbarTitle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Treeview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/TreeviewNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/VirtualTable.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/VuetifyWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/Window.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/WindowItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-04 16:07:24.000000 ipyvuetify-1.8.8/ipyvuetify/generated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.532258 ipyvuetify-1.8.8/ipyvuetify/labextension/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2534 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.540258 ipyvuetify-1.8.8/ipyvuetify/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/010c1aeee3c6d1cbb1d5761d80353823.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/037d830416495def72b7881024c14b7b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/0509ab09c1b0d2200a4135803c91d6ce.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   638476 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js
--rw-r--r--   0 runner    (1001) docker     (123)    91293 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/18.65b4e6d7bbb837a6285e.js
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21776 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/210a7c781f5a354a0e4985656ab456d9.woff
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/261.f67c431b049461460d89.js
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/285467176f7fe6bb6a9c6873b3dad2cc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/29b882f018fa6fe75fd338aaae6235b8.woff
--rw-r--r--   0 runner    (1001) docker     (123)   844600 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/2d0a0d8f5f173be15a67aa084db94fe6.eot
--rw-r--r--   0 runner    (1001) docker     (123)   974057 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/353.3d1742277c7640de5c75.js
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/510dec37fa69fba39593e01a469ee018.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/55536c8e9e9a532651e3cf374f290ea3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/6232f43d15b0e7a0bf0fe82e295bdd06.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/635.ba9631c2c215c7a91978.js
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/701.cbac5919a0796529305e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/7b770d6c53423deb1a8e49d3c9175184.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/846d1890aee87fde5d8ced8eba360c3a.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/8c2ade503b34e31430d6c98aa29a52a3.woff
--rw-r--r--   0 runner    (1001) docker     (123)   150680 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/925.f89c57337496b4532b48.js
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/9680d5a0c32d2fd084e07bbc4c8b2923.woff
--rw-r--r--   0 runner    (1001) docker     (123)    69177 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/96c476804d7a788cc1c05351b287ee41.eot
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/987b84570ea69ee660455b8d5e91f5f1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/a1471d1d6431c893582a5f6a250db3f9.woff
--rw-r--r--   0 runner    (1001) docker     (123)   404384 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/b4917be25082eb793b5363f2fdb5f282.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/bafb105baeb22d965c70fe52ba6b49d9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/bc833e725c137257c2c42a789845d82f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/cf6613d1adf490972c557a8e318e0868.woff
--rw-r--r--   0 runner    (1001) docker     (123)   283040 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/d69924b98acd849cdeba9fbff3f88ea6.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/d704bb3d579b7d5e40880c75705c8a71.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   174048 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/da4ea5cdfca6b3baab285741f5ccb59f.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/de8b7431b74642e830af4d4f4b513ec9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/e9dbbe8a693dd275c16d32feb101f1c1.woff
--rw-r--r--   0 runner    (1001) docker     (123)   844380 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/f51112347be6b44f9ef46151a971430d.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-04 16:08:07.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/remoteEntry.4682de76162aa455d184.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 16:07:54.000000 ipyvuetify-1.8.8/ipyvuetify/labextension/static/style.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.556258 ipyvuetify-1.8.8/ipyvuetify/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/010c1aeee3c6d1cbb1d5761d80353823.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/037d830416495def72b7881024c14b7b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/0509ab09c1b0d2200a4135803c91d6ce.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21776 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/210a7c781f5a354a0e4985656ab456d9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/285467176f7fe6bb6a9c6873b3dad2cc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/29b882f018fa6fe75fd338aaae6235b8.woff
--rw-r--r--   0 runner    (1001) docker     (123)   844600 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/2d0a0d8f5f173be15a67aa084db94fe6.eot
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/510dec37fa69fba39593e01a469ee018.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/55536c8e9e9a532651e3cf374f290ea3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/6232f43d15b0e7a0bf0fe82e295bdd06.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/7b770d6c53423deb1a8e49d3c9175184.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/846d1890aee87fde5d8ced8eba360c3a.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/8c2ade503b34e31430d6c98aa29a52a3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/9680d5a0c32d2fd084e07bbc4c8b2923.woff
--rw-r--r--   0 runner    (1001) docker     (123)    69177 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/96c476804d7a788cc1c05351b287ee41.eot
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/987b84570ea69ee660455b8d5e91f5f1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/a1471d1d6431c893582a5f6a250db3f9.woff
--rw-r--r--   0 runner    (1001) docker     (123)   404384 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/b4917be25082eb793b5363f2fdb5f282.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/bafb105baeb22d965c70fe52ba6b49d9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/bc833e725c137257c2c42a789845d82f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/cf6613d1adf490972c557a8e318e0868.woff
--rw-r--r--   0 runner    (1001) docker     (123)   283040 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/d69924b98acd849cdeba9fbff3f88ea6.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/d704bb3d579b7d5e40880c75705c8a71.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   174048 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/da4ea5cdfca6b3baab285741f5ccb59f.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/de8b7431b74642e830af4d4f4b513ec9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 16:08:39.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/e9dbbe8a693dd275c16d32feb101f1c1.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-04 16:08:10.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)   844380 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/f51112347be6b44f9ef46151a971430d.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff
--rw-r--r--   0 runner    (1001) docker     (123)  1890961 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)  3823725 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   182750 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/nodeps.js
--rw-r--r--   0 runner    (1001) docker     (123)   539676 2023-04-04 16:08:40.000000 ipyvuetify-1.8.8/ipyvuetify/nbextension/nodeps.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:42.512257 ipyvuetify-1.8.8/ipyvuetify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 16:08:42.000000 ipyvuetify-1.8.8/ipyvuetify.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/jupyter-vuetify.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-04 16:08:42.560258 ipyvuetify-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-04 16:06:31.000000 ipyvuetify-1.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.706674 ipyvuetify-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 19:21:01.706674 ipyvuetify-1.8.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5680 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.642673 ipyvuetify-1.8.9/ipyvuetify/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/Html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/Themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/VuetifyTemplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.642673 ipyvuetify-1.8.9/ipyvuetify/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/extra/file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/ipyvuetify/extra/file_input.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.670673 ipyvuetify-1.8.9/ipyvuetify/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/App.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/AppBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/AppBarNavIcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Avatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/BottomNavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/BottomSheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Breadcrumbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/BreadcrumbsDivider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/BreadcrumbsItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/BtnToggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CalendarDaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CalendarMonthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CalendarWeekly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CardActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CardSubtitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CardText.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CardTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Carousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CarouselItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CarouselReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/CarouselTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ChipGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ColorPicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ColorPickerCanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ColorPickerSwatches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DataFooter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DataIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DataTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DataTableHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerDateTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerMonthTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerYears.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DialogBottomTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/DialogTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/EditDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpandTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpandXTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanelContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanelHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/FabTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/FadeTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/FileInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Hover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ItemGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/List.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemActionText.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemAvatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemIcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemSubtitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ListItemTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/MenuTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/NavigationDrawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/OverflowBtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Parallax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ProgressCircular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ProgressLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/RadioGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/RangeSlider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ScaleTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ScrollXReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ScrollXTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ScrollYReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ScrollYTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SimpleCheckbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SimpleTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SkeletonLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideXReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideXTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideYReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SlideYTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Snackbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SpeedDial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/StepperContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/StepperHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/StepperItems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/StepperStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Subheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/SystemBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TabItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TabReverseTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TabTransition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TableOverflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TabsItems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TabsSlider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TextField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Textarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ThemeProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TimePicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TimePickerClock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TimePickerTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TimelineItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ToolbarItems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/ToolbarTitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Treeview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/TreeviewNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/VirtualTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/VuetifyWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/Window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/WindowItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-04 19:19:28.000000 ipyvuetify-1.8.9/ipyvuetify/generated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.670673 ipyvuetify-1.8.9/ipyvuetify/labextension/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2534 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.682674 ipyvuetify-1.8.9/ipyvuetify/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/010c1aeee3c6d1cbb1d5761d80353823.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/037d830416495def72b7881024c14b7b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/0509ab09c1b0d2200a4135803c91d6ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   638476 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91293 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/18.65b4e6d7bbb837a6285e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21776 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/210a7c781f5a354a0e4985656ab456d9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/261.f67c431b049461460d89.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/285467176f7fe6bb6a9c6873b3dad2cc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/29b882f018fa6fe75fd338aaae6235b8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   844600 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/2d0a0d8f5f173be15a67aa084db94fe6.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   974057 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/353.3d1742277c7640de5c75.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/510dec37fa69fba39593e01a469ee018.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/55536c8e9e9a532651e3cf374f290ea3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/6232f43d15b0e7a0bf0fe82e295bdd06.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/635.ba9631c2c215c7a91978.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/701.cbac5919a0796529305e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/7b770d6c53423deb1a8e49d3c9175184.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/846d1890aee87fde5d8ced8eba360c3a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/8c2ade503b34e31430d6c98aa29a52a3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   150680 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/925.303122e70cd86f1083f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/9680d5a0c32d2fd084e07bbc4c8b2923.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    69177 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/96c476804d7a788cc1c05351b287ee41.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/987b84570ea69ee660455b8d5e91f5f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/a1471d1d6431c893582a5f6a250db3f9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   404384 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/b4917be25082eb793b5363f2fdb5f282.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/bafb105baeb22d965c70fe52ba6b49d9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/bc833e725c137257c2c42a789845d82f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/cf6613d1adf490972c557a8e318e0868.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   283040 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/d69924b98acd849cdeba9fbff3f88ea6.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/d704bb3d579b7d5e40880c75705c8a71.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   174048 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/da4ea5cdfca6b3baab285741f5ccb59f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/de8b7431b74642e830af4d4f4b513ec9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/e9dbbe8a693dd275c16d32feb101f1c1.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   844380 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/f51112347be6b44f9ef46151a971430d.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-04 19:20:20.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/remoteEntry.48ed45d1d2602f161365.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-04 19:20:04.000000 ipyvuetify-1.8.9/ipyvuetify/labextension/static/style.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.702674 ipyvuetify-1.8.9/ipyvuetify/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16572 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/010c1aeee3c6d1cbb1d5761d80353823.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/037d830416495def72b7881024c14b7b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/0509ab09c1b0d2200a4135803c91d6ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21776 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/210a7c781f5a354a0e4985656ab456d9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/285467176f7fe6bb6a9c6873b3dad2cc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/29b882f018fa6fe75fd338aaae6235b8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   844600 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/2d0a0d8f5f173be15a67aa084db94fe6.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/510dec37fa69fba39593e01a469ee018.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/55536c8e9e9a532651e3cf374f290ea3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/6232f43d15b0e7a0bf0fe82e295bdd06.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/7b770d6c53423deb1a8e49d3c9175184.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/846d1890aee87fde5d8ced8eba360c3a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/8c2ade503b34e31430d6c98aa29a52a3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/9680d5a0c32d2fd084e07bbc4c8b2923.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    69177 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/96c476804d7a788cc1c05351b287ee41.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/987b84570ea69ee660455b8d5e91f5f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/a1471d1d6431c893582a5f6a250db3f9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   404384 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/b4917be25082eb793b5363f2fdb5f282.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/bafb105baeb22d965c70fe52ba6b49d9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/bc833e725c137257c2c42a789845d82f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/cf6613d1adf490972c557a8e318e0868.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   283040 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/d69924b98acd849cdeba9fbff3f88ea6.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/d704bb3d579b7d5e40880c75705c8a71.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   174048 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/da4ea5cdfca6b3baab285741f5ccb59f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/de8b7431b74642e830af4d4f4b513ec9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/e9dbbe8a693dd275c16d32feb101f1c1.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-04 19:20:23.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)   844380 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/f51112347be6b44f9ef46151a971430d.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  1890961 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3823725 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   182750 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/nodeps.js
+-rw-r--r--   0 runner    (1001) docker     (123)   539676 2023-04-04 19:20:59.000000 ipyvuetify-1.8.9/ipyvuetify/nbextension/nodeps.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:21:01.642673 ipyvuetify-1.8.9/ipyvuetify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 19:21:01.000000 ipyvuetify-1.8.9/ipyvuetify.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/jupyter-vuetify.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-04 19:21:01.706674 ipyvuetify-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-04 19:18:27.000000 ipyvuetify-1.8.9/setup.py
```

### Comparing `ipyvuetify-1.8.8/LICENSE` & `ipyvuetify-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/PKG-INFO` & `ipyvuetify-1.8.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvuetify
-Version: 1.8.8
+Version: 1.8.9
 Summary: Jupyter widgets based on vuetify UI components
 Home-page: https://github.com/widgetti/ipyvuetify
 Author: Mario Buikhuizen, Maarten Breddels
 Author-email: mbuikhuizen@gmail.com, maartenbreddels@gmail.com
 Keywords: ipython,jupyter,widgets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ipyvuetify-1.8.8/README.md` & `ipyvuetify-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/Html.py` & `ipyvuetify-1.8.9/ipyvuetify/Html.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/Themes.py` & `ipyvuetify-1.8.9/ipyvuetify/Themes.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/VuetifyTemplate.py` & `ipyvuetify-1.8.9/ipyvuetify/VuetifyTemplate.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/__init__.py` & `ipyvuetify-1.8.9/ipyvuetify/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/extra/file_input.py` & `ipyvuetify-1.8.9/ipyvuetify/extra/file_input.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/extra/file_input.vue` & `ipyvuetify-1.8.9/ipyvuetify/extra/file_input.vue`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Alert.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Alert.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/AppBar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/AppBar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Autocomplete.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Autocomplete.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Avatar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Avatar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Badge.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Badge.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Banner.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Banner.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/BottomNavigation.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/BottomNavigation.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/BottomSheet.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/BottomSheet.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Breadcrumbs.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/BreadcrumbsItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/BreadcrumbsItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Btn.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Btn.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/BtnToggle.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/BtnToggle.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Calendar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Calendar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CalendarDaily.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CalendarDaily.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CalendarMonthly.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CalendarMonthly.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CalendarWeekly.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CalendarWeekly.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Card.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Card.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Carousel.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Carousel.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CarouselItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CarouselItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CarouselReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CarouselReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/CarouselTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/CarouselTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Checkbox.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Checkbox.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Chip.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Chip.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ChipGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ChipGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Col.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Col.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ColorPicker.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ColorPicker.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ColorPickerCanvas.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ColorPickerCanvas.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ColorPickerSwatches.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ColorPickerSwatches.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Combobox.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Combobox.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Container.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Container.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Content.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Content.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Counter.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Counter.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Data.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Data.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DataFooter.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DataFooter.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DataIterator.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DataIterator.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DataTable.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DataTable.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePicker.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePicker.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerDateTable.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerDateTable.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerHeader.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerHeader.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerMonthTable.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerMonthTable.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerTitle.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerTitle.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DatePickerYears.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DatePickerYears.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Dialog.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Dialog.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DialogBottomTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DialogBottomTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/DialogTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/DialogTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/EditDialog.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/EditDialog.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanelHeader.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanelHeader.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ExpansionPanels.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ExpansionPanels.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/FabTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/FabTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/FadeTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/FadeTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/FileInput.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/FileInput.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Flex.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Flex.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Footer.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Footer.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Hover.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Hover.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Icon.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Icon.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Img.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Img.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Input.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Input.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ItemGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ItemGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Label.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Label.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Layout.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Layout.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Lazy.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Lazy.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/List.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/List.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ListGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ListGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ListItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ListItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ListItemAvatar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ListItemAvatar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ListItemGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ListItemGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Menu.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Menu.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/MenuTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/MenuTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Messages.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Messages.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/NavigationDrawer.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/NavigationDrawer.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/OverflowBtn.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/OverflowBtn.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Overlay.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Overlay.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Pagination.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Pagination.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Picker.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Picker.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ProgressCircular.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ProgressCircular.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ProgressLinear.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ProgressLinear.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Radio.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Radio.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/RadioGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/RadioGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/RangeSlider.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/RangeSlider.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Rating.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Rating.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Responsive.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Responsive.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Row.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Row.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ScaleTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ScaleTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ScrollXReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ScrollXReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ScrollXTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ScrollXTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ScrollYReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ScrollYReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/ScrollYTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/ScrollYTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Select.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Select.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Sheet.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Sheet.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SimpleCheckbox.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SimpleCheckbox.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SimpleTable.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SimpleTable.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SkeletonLoader.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SkeletonLoader.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SlideGroup.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SlideGroup.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SlideXReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SlideXReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SlideXTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SlideXTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SlideYReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SlideYReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SlideYTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SlideYTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Slider.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Slider.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Snackbar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Snackbar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Sparkline.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Sparkline.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SpeedDial.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SpeedDial.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Stepper.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Stepper.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/StepperStep.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/StepperStep.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Switch.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Switch.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/SystemBar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/SystemBar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Tab.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Tab.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TabItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TabItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TabReverseTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TabReverseTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TabTransition.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TabTransition.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Tabs.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Tabs.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TabsItems.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TabsItems.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TextField.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TextField.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Textarea.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Textarea.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TimePicker.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TimePicker.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TimePickerClock.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TimePickerClock.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TimePickerTitle.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TimePickerTitle.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Timeline.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Timeline.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TimelineItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TimelineItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Toolbar.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Toolbar.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Tooltip.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Tooltip.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Treeview.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Treeview.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/TreeviewNode.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/TreeviewNode.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/VirtualTable.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/VirtualTable.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/VuetifyWidget.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/VuetifyWidget.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/Window.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/Window.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/WindowItem.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/WindowItem.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/generated/__init__.py` & `ipyvuetify-1.8.9/ipyvuetify/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/package.json` & `ipyvuetify-1.8.9/ipyvuetify/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9633928571428572%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.48ed45d1d2602f161365.js'}}",*

 * * "'version'": "'1.8.9'"}*

```diff
@@ -36,15 +36,15 @@
         "lib/**/*.js",
         "dist/",
         "styles.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4682de76162aa455d184.js"
+            "load": "static/remoteEntry.48ed45d1d2602f161365.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../ipyvuetify/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -82,9 +82,9 @@
         "prepare": "run-s build:*",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "run-p watch:*",
         "watch:babel": "babel src --watch --out-dir lib --copy-files --verbose",
         "watch:labextension": "jupyter labextension watch .",
         "watch:webpack": "webpack --mode development --watch"
     },
-    "version": "1.8.8"
+    "version": "1.8.9"
 }
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/010c1aeee3c6d1cbb1d5761d80353823.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/010c1aeee3c6d1cbb1d5761d80353823.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/037d830416495def72b7881024c14b7b.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/037d830416495def72b7881024c14b7b.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/0509ab09c1b0d2200a4135803c91d6ce.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/0509ab09c1b0d2200a4135803c91d6ce.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js.LICENSE.txt` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/102.602144dedc889a9e2f01.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/18.65b4e6d7bbb837a6285e.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/18.65b4e6d7bbb837a6285e.js`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/210a7c781f5a354a0e4985656ab456d9.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/210a7c781f5a354a0e4985656ab456d9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/285467176f7fe6bb6a9c6873b3dad2cc.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/285467176f7fe6bb6a9c6873b3dad2cc.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/29b882f018fa6fe75fd338aaae6235b8.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/29b882f018fa6fe75fd338aaae6235b8.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/2d0a0d8f5f173be15a67aa084db94fe6.eot` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/2d0a0d8f5f173be15a67aa084db94fe6.eot`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/353.3d1742277c7640de5c75.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/353.3d1742277c7640de5c75.js`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/510dec37fa69fba39593e01a469ee018.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/510dec37fa69fba39593e01a469ee018.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/55536c8e9e9a532651e3cf374f290ea3.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/55536c8e9e9a532651e3cf374f290ea3.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/6232f43d15b0e7a0bf0fe82e295bdd06.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/6232f43d15b0e7a0bf0fe82e295bdd06.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/701.cbac5919a0796529305e.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/701.cbac5919a0796529305e.js`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/7b770d6c53423deb1a8e49d3c9175184.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/7b770d6c53423deb1a8e49d3c9175184.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/846d1890aee87fde5d8ced8eba360c3a.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/846d1890aee87fde5d8ced8eba360c3a.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/8c2ade503b34e31430d6c98aa29a52a3.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/8c2ade503b34e31430d6c98aa29a52a3.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/925.f89c57337496b4532b48.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/925.303122e70cd86f1083f8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8510,11 +8510,11 @@
                 hmr: !0,
                 transform: void 0,
                 insertInto: void 0
             }), t.locals && (e.exports = t.locals)
         },
         306: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"jupyter-vuetify","version":"1.8.8","description":"Jupyter widgets based on vuetify UI components","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvuetify.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/**/*.js","lib/**/*.js","dist/","styles.css"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^2.1.1","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^3.0.1","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^4.31.0","webpack-cli":"^3.3.2"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@jupyterlab/apputils":"^2 || ^3","@mariobuikhuizen/vuetify":"2.2.26-rc.0","@mdi/font":"^4.9.95","core-js":"^3.0.1","jupyter-vue":"^1.0.0","lodash":"^4.17.11","material-design-icons-iconfont":"^5.0.1","typeface-roboto":"0.0.54"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvuetify/labextension","webpackConfig":"webpack.config.lab3.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/apputils":{"bundled":false,"singleton":true},"jupyter-vue":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"jupyter-vuetify","version":"1.8.9","description":"Jupyter widgets based on vuetify UI components","license":"MIT","author":"Mario Buikhuizen, Maarten Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/mariobuikhuizen/ipyvuetify.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["src/**/*.js","lib/**/*.js","dist/","styles.css"],"browserslist":">0.8%, not ie 11, not op_mini all, not dead","scripts":{"build:babel":"babel src --out-dir lib --copy-files","watch:babel":"babel src --watch --out-dir lib --copy-files --verbose","build:labextension":"jupyter labextension build .","watch:labextension":"jupyter labextension watch .","build:webpack":"webpack","watch:webpack":"webpack --mode development --watch","watch":"run-p watch:*","clean":"rimraf lib/ dist/","prepare":"run-s build:*","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@babel/cli":"^7.5.0","@babel/core":"^7.4.4","@babel/preset-env":"^7.4.4","@jupyterlab/builder":"^3","ajv":"^6.10.0","css-loader":"^2.1.1","eslint":"^5.16.0","eslint-config-airbnb-base":"^13.1.0","eslint-plugin-import":"^2.17.2","eslint-plugin-vue":"^5.2.2","file-loader":"^3.0.1","npm-run-all":"^4.1.5","rimraf":"^2.6.3","style-loader":"^0.23.1","webpack":"^4.31.0","webpack-cli":"^3.3.2"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2 || ^3 || ^4","@jupyterlab/apputils":"^2 || ^3","@mariobuikhuizen/vuetify":"2.2.26-rc.0","@mdi/font":"^4.9.95","core-js":"^3.0.1","jupyter-vue":"^1.0.0","lodash":"^4.17.11","material-design-icons-iconfont":"^5.0.1","typeface-roboto":"0.0.54"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../ipyvuetify/labextension","webpackConfig":"webpack.config.lab3.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@jupyterlab/apputils":{"bundled":false,"singleton":true},"jupyter-vue":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/9680d5a0c32d2fd084e07bbc4c8b2923.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/9680d5a0c32d2fd084e07bbc4c8b2923.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/96c476804d7a788cc1c05351b287ee41.eot` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/96c476804d7a788cc1c05351b287ee41.eot`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/987b84570ea69ee660455b8d5e91f5f1.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/987b84570ea69ee660455b8d5e91f5f1.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/a1471d1d6431c893582a5f6a250db3f9.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/a1471d1d6431c893582a5f6a250db3f9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/b4917be25082eb793b5363f2fdb5f282.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/b4917be25082eb793b5363f2fdb5f282.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/bafb105baeb22d965c70fe52ba6b49d9.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/bafb105baeb22d965c70fe52ba6b49d9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/bc833e725c137257c2c42a789845d82f.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/bc833e725c137257c2c42a789845d82f.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/cf6613d1adf490972c557a8e318e0868.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/cf6613d1adf490972c557a8e318e0868.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/d69924b98acd849cdeba9fbff3f88ea6.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/d69924b98acd849cdeba9fbff3f88ea6.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/d704bb3d579b7d5e40880c75705c8a71.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/d704bb3d579b7d5e40880c75705c8a71.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/da4ea5cdfca6b3baab285741f5ccb59f.ttf` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/da4ea5cdfca6b3baab285741f5ccb59f.ttf`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/de8b7431b74642e830af4d4f4b513ec9.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/de8b7431b74642e830af4d4f4b513ec9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/e9dbbe8a693dd275c16d32feb101f1c1.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/e9dbbe8a693dd275c16d32feb101f1c1.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/f51112347be6b44f9ef46151a971430d.ttf` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/f51112347be6b44f9ef46151a971430d.ttf`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/labextension/static/remoteEntry.4682de76162aa455d184.js` & `ipyvuetify-1.8.9/ipyvuetify/labextension/static/remoteEntry.48ed45d1d2602f161365.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -48,15 +48,15 @@
         18: "65b4e6d7bbb837a6285e",
         102: "602144dedc889a9e2f01",
         215: "d31a68f64db81d7974d7",
         261: "f67c431b049461460d89",
         353: "3d1742277c7640de5c75",
         635: "ba9631c2c215c7a91978",
         701: "cbac5919a0796529305e",
-        925: "f89c57337496b4532b48"
+        925: "303122e70cd86f1083f8"
     } [e] + ".js", w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -109,15 +109,15 @@
                             get: t,
                             from: i
                         })
                     },
                     l = [];
                 switch (t) {
                     case "default":
-                        u("@mariobuikhuizen/vuetify", "2.2.26-rc.0", (() => Promise.all([w.e(102), w.e(215), w.e(635)]).then((() => () => w(8102))))), u("jupyter-vuetify", "1.8.8", (() => Promise.all([w.e(353), w.e(215), w.e(925)]).then((() => () => w(6925))))), u("typeface-roboto", "0.0.54", (() => w.e(701).then((() => () => w(701)))))
+                        u("@mariobuikhuizen/vuetify", "2.2.26-rc.0", (() => Promise.all([w.e(102), w.e(215), w.e(635)]).then((() => () => w(8102))))), u("jupyter-vuetify", "1.8.9", (() => Promise.all([w.e(353), w.e(215), w.e(925)]).then((() => () => w(6925))))), u("typeface-roboto", "0.0.54", (() => w.e(701).then((() => () => w(701)))))
                 }
                 return e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/010c1aeee3c6d1cbb1d5761d80353823.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/010c1aeee3c6d1cbb1d5761d80353823.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/037d830416495def72b7881024c14b7b.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/037d830416495def72b7881024c14b7b.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/0509ab09c1b0d2200a4135803c91d6ce.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/0509ab09c1b0d2200a4135803c91d6ce.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/210a7c781f5a354a0e4985656ab456d9.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/210a7c781f5a354a0e4985656ab456d9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/285467176f7fe6bb6a9c6873b3dad2cc.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/285467176f7fe6bb6a9c6873b3dad2cc.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/29b882f018fa6fe75fd338aaae6235b8.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/29b882f018fa6fe75fd338aaae6235b8.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/2d0a0d8f5f173be15a67aa084db94fe6.eot` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/2d0a0d8f5f173be15a67aa084db94fe6.eot`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/510dec37fa69fba39593e01a469ee018.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/510dec37fa69fba39593e01a469ee018.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/55536c8e9e9a532651e3cf374f290ea3.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/55536c8e9e9a532651e3cf374f290ea3.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/6232f43d15b0e7a0bf0fe82e295bdd06.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/6232f43d15b0e7a0bf0fe82e295bdd06.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/7b770d6c53423deb1a8e49d3c9175184.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/7b770d6c53423deb1a8e49d3c9175184.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/846d1890aee87fde5d8ced8eba360c3a.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/846d1890aee87fde5d8ced8eba360c3a.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/8c2ade503b34e31430d6c98aa29a52a3.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/8c2ade503b34e31430d6c98aa29a52a3.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/9680d5a0c32d2fd084e07bbc4c8b2923.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/9680d5a0c32d2fd084e07bbc4c8b2923.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/96c476804d7a788cc1c05351b287ee41.eot` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/96c476804d7a788cc1c05351b287ee41.eot`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/987b84570ea69ee660455b8d5e91f5f1.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/987b84570ea69ee660455b8d5e91f5f1.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/a1471d1d6431c893582a5f6a250db3f9.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/a1471d1d6431c893582a5f6a250db3f9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/b4917be25082eb793b5363f2fdb5f282.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/b4917be25082eb793b5363f2fdb5f282.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/bafb105baeb22d965c70fe52ba6b49d9.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/bafb105baeb22d965c70fe52ba6b49d9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/bc833e725c137257c2c42a789845d82f.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/bc833e725c137257c2c42a789845d82f.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/cf6613d1adf490972c557a8e318e0868.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/cf6613d1adf490972c557a8e318e0868.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/d0066537ab6a4c6f8285a5aeb3ba5f09.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/d69924b98acd849cdeba9fbff3f88ea6.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/d69924b98acd849cdeba9fbff3f88ea6.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/d704bb3d579b7d5e40880c75705c8a71.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/d704bb3d579b7d5e40880c75705c8a71.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/da4ea5cdfca6b3baab285741f5ccb59f.ttf` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/da4ea5cdfca6b3baab285741f5ccb59f.ttf`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/de8b7431b74642e830af4d4f4b513ec9.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/de8b7431b74642e830af4d4f4b513ec9.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/e9dbbe8a693dd275c16d32feb101f1c1.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/e9dbbe8a693dd275c16d32feb101f1c1.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/extension.js` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/f51112347be6b44f9ef46151a971430d.ttf` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/f51112347be6b44f9ef46151a971430d.ttf`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/index.js` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -32047,15 +32047,15 @@
             TextTrackCueList: 0,
             TextTrackList: 0,
             TouchList: 0
         }
     }, function(e) {
         e.exports = {
             name: "jupyter-vuetify",
-            version: "1.8.8",
+            version: "1.8.9",
             description: "Jupyter widgets based on vuetify UI components",
             license: "MIT",
             author: "Mario Buikhuizen, Maarten Breddels",
             main: "lib/index.js",
             repository: {
                 type: "git",
                 url: "https://github.com/mariobuikhuizen/ipyvuetify.git"
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/index.js.map` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/nodeps.js` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/nodeps.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1188,15 +1188,15 @@
             TextTrackCueList: 0,
             TextTrackList: 0,
             TouchList: 0
         }
     }, function(e) {
         e.exports = {
             name: "jupyter-vuetify",
-            version: "1.8.8",
+            version: "1.8.9",
             description: "Jupyter widgets based on vuetify UI components",
             license: "MIT",
             author: "Mario Buikhuizen, Maarten Breddels",
             main: "lib/index.js",
             repository: {
                 type: "git",
                 url: "https://github.com/mariobuikhuizen/ipyvuetify.git"
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify/nbextension/nodeps.js.map` & `ipyvuetify-1.8.9/ipyvuetify/nbextension/nodeps.js.map`

 * *Files identical despite different names*

### Comparing `ipyvuetify-1.8.8/ipyvuetify.egg-info/PKG-INFO` & `ipyvuetify-1.8.9/ipyvuetify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvuetify
-Version: 1.8.8
+Version: 1.8.9
 Summary: Jupyter widgets based on vuetify UI components
 Home-page: https://github.com/widgetti/ipyvuetify
 Author: Mario Buikhuizen, Maarten Breddels
 Author-email: mbuikhuizen@gmail.com, maartenbreddels@gmail.com
 Keywords: ipython,jupyter,widgets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ipyvuetify-1.8.8/ipyvuetify.egg-info/SOURCES.txt` & `ipyvuetify-1.8.9/ipyvuetify.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 ipyvuetify/labextension/static/5d4aeb4e5f5ef754e307d7ffaef688bd.woff2
 ipyvuetify/labextension/static/6232f43d15b0e7a0bf0fe82e295bdd06.woff2
 ipyvuetify/labextension/static/635.ba9631c2c215c7a91978.js
 ipyvuetify/labextension/static/701.cbac5919a0796529305e.js
 ipyvuetify/labextension/static/7b770d6c53423deb1a8e49d3c9175184.woff2
 ipyvuetify/labextension/static/846d1890aee87fde5d8ced8eba360c3a.woff
 ipyvuetify/labextension/static/8c2ade503b34e31430d6c98aa29a52a3.woff
-ipyvuetify/labextension/static/925.f89c57337496b4532b48.js
+ipyvuetify/labextension/static/925.303122e70cd86f1083f8.js
 ipyvuetify/labextension/static/9680d5a0c32d2fd084e07bbc4c8b2923.woff
 ipyvuetify/labextension/static/96c476804d7a788cc1c05351b287ee41.eot
 ipyvuetify/labextension/static/987b84570ea69ee660455b8d5e91f5f1.woff2
 ipyvuetify/labextension/static/a1471d1d6431c893582a5f6a250db3f9.woff
 ipyvuetify/labextension/static/b4917be25082eb793b5363f2fdb5f282.woff
 ipyvuetify/labextension/static/bafb105baeb22d965c70fe52ba6b49d9.woff
 ipyvuetify/labextension/static/bc833e725c137257c2c42a789845d82f.woff
@@ -217,15 +217,15 @@
 ipyvuetify/labextension/static/d704bb3d579b7d5e40880c75705c8a71.woff
 ipyvuetify/labextension/static/d8bcbe724fd6f4ba44d0ee6a2675890f.woff2
 ipyvuetify/labextension/static/da4ea5cdfca6b3baab285741f5ccb59f.ttf
 ipyvuetify/labextension/static/de8b7431b74642e830af4d4f4b513ec9.woff
 ipyvuetify/labextension/static/e9dbbe8a693dd275c16d32feb101f1c1.woff
 ipyvuetify/labextension/static/f51112347be6b44f9ef46151a971430d.ttf
 ipyvuetify/labextension/static/ffcc050b2d92d4b14a4fcb527ee0bcc8.woff
-ipyvuetify/labextension/static/remoteEntry.4682de76162aa455d184.js
+ipyvuetify/labextension/static/remoteEntry.48ed45d1d2602f161365.js
 ipyvuetify/labextension/static/style.js
 ipyvuetify/nbextension/010c1aeee3c6d1cbb1d5761d80353823.woff2
 ipyvuetify/nbextension/037d830416495def72b7881024c14b7b.woff2
 ipyvuetify/nbextension/0509ab09c1b0d2200a4135803c91d6ce.woff2
 ipyvuetify/nbextension/19b7a0adfdd4f808b53af7e2ce2ad4e5.woff2
 ipyvuetify/nbextension/210a7c781f5a354a0e4985656ab456d9.woff
 ipyvuetify/nbextension/285467176f7fe6bb6a9c6873b3dad2cc.woff2
```

### Comparing `ipyvuetify-1.8.8/setup.py` & `ipyvuetify-1.8.9/setup.py`

 * *Files identical despite different names*

