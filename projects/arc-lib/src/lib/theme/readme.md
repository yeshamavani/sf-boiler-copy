# THEME MODULE

- Theme module in the boilerplate is usually used in conjunction with Nebular,Nebular is a customizable Angular UI Library and styles designed to create a consistent, modern user interface. Nebular includes a set of pre-defined themes, but you can also create your own custom themes also.

## IconPacksManagerService

- `IconPacksManagerService` that is used to manage and register various icon packs for an Angular application that is using the Nebular theme library.

- The service class imports the `NbIconLibraries` class from the Nebular theme library and the      
 `ThemeModule` from the application's theme module. It also imports SVG icons which are presumably used in the application. & also we can add custum SVG icons and modify accordingly as per user needs
 The service class has three methods:

-  `registerFontAwesome()` which registers the `font-awesome` icon pack using the `registerFontPack()` 
    method of `NbIconLibraries`. The iconClassPrefix "fa" is provided as a parameter which will be used to prefix all icon classes in the `font-awesome` pack.

-  `registerPack(name, params)` which registers a custom icon pack with the provided name and parameters 
    using the `registerFontPack()` method of `NbIconLibraries`. The "params" object is an optional parameter which contains the `iconClassPrefix`.

-  `registerSvgs()` which registers a custom SVG icon pack called `svg-boiler` using the `registerSvgPack()`
    method of `NbIconLibraries`. The pack contains SVG icon "kebab", which are passed as objects to the `registerSvgPack()` method.

#### Styles

- In styles boilerplate have all the files which The boilerplate using for styling and designing the data 
  in presentable way for this The boilerplate usingthese files named `mixins`,`utilities`,`variables` and `dhtmlx_gantt` These all are the collection of Sass files can be used to quickly add styles to HTML elements.for example The boilerplate using `padding,width,height,margin,color-cases,font-size,alignment` etc.

## Toaster

### ToasterService:

We are using `ToasterService` that provides methods to display toasts using the `NbToastrService` and
The `ToasterService` provides the methods to show different types of toasts like :
- `show`: shows a generic toast.
- `success`: shows a success toast.
- `info`: shows an info toast .
- `warn`: shows a warning toast.
- `error`: shows an error toast .
  Each of these methods takes a message and an optional title, and a configuration object that can be used to customize the appearance and behavior of the toast.

### ToasterAdapterService:

In boilerplate `ToasterAdapterService` implements the `IAdapter` interface for converting between two different types of objects: `ToasterConfigExt` and `NbToastrConfig`.

- `ngx-toastr` which provides a toast notification service for Angular applications. It allows you to configure various options for the toast notifications, including their appearance, position, duration, and behavior. The library provides a `ToastrConfig` class that you can use to set these options globally for your application or on a per-toast basis.

- `NbToastrConfig` is a configuration service provided by the Nebular UI library, which is used to customize the appearance and behavior of toast notifications.
