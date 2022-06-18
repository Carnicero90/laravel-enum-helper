![Enum Helper-Dark](branding/laravel-dark.png#gh-dark-mode-only)![Enum Helper-Light](branding/laravel-light.png#gh-light-mode-only)
# Enum Helper
[![Latest Version on Packagist](https://img.shields.io/packagist/v/datomatic/laravel-enum-helper.svg?style=for-the-badge)](https://packagist.org/packages/datomatic/laravel-enum-helper)
[![Pest Tests number](https://img.shields.io/static/v1?label=%23tests&message=56&color=FF88FA&style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAcCAMAAABF0y+mAAABiVBMVEUAAAD/iPv9yP3Xm+j/mP//wfVj67Je6bP/h/pVx6p6175d57WQycf+iPn/iPrsnezArd3+t/qpvNJd6LP/jPpu6rv/lPr/kPpc57T/rvtc57Np6rj3oPl37cL/tfn/wv9d6brX//L/g/rYn+n/gvrWm+di6LX+jPrskfGWzMpt6bln4bdd57Jk6LWSycj+vPquwNVo6rde6bP7nvvYnup91b/+vfv/lvtc57OqvNTFs9//t/td57L9t/r/iPpd6LPapej/ovp26bxy67v9lfld6LJr4Ljwsvb/xv3/jv39zv1t6buG5cTDreH5ivlc5rJy676V4cxb57D/y/h50MOy4OCUxcVa77X/iPpe6LP/jP+pu9L8t///tvuQycfArNxp6LzArd151r7/i/9n4bb/j/9e6rT/ifr7ifrskvLYnuhi87tg8blg7bf/vv//lP+wxNtj9b3/qv//oP/+ivz/l/r8ifryn/fvlPTfpPDeofDKtujHtOWX1NF/4seC3cR82sFu7cBo5LiMwPMrAAAAWHRSTlMA/Wv8FAIC/dME/Wj+3tEG/Pv798G1oHRjS0k1LBsWDgsJ/v36+fTy8ezn4+Lh29XNzMzLysLAwLSwr66opJqakY+Ni4J7end0bGlpY11XU048KicmIR8fizl+vwAAAVdJREFUKM9tz2VXAlEQgOFBBURpkE67u7u7E1YFYQl1SbvrlztDiLvss+fc/fCemXMvAEhhKqU759P1rLoxUDUyEh9fPH0z7ALiVrEY+SSNtxNS2upouYv7hOL191aKVsZHUTgbnQPQgDkq4ctHdoQmTWmW4WFzlVUDVpNKXf2fWpWbZIwUq/hcmjWGYnSa1pZZjEoomrEdVAisD7CX6GEb40rqTODxCj21OjDOvjRV8l2jhudBDchg/FUbDIZCITzwQyH6a9+2AMDbm9GfltFnxgAdtQWUgQJl4VQq37uPcSnsfYZzav6Ew18fQ4fUYPM7Qn4uSiIdyx5saJ6T+/3+5KSltshicwI2UpfAKE/aoARTvnn7KMYMdlAUyWRSyHN2JeU42HlCi4TszTHcmuj3iMVdP5JzoyAWNzi6T3ZGrMFCliK3BAqRSC/B2+6IxvYYNcO+2Npfv+yFi10LfBUAAAAASUVORK5CYII=)](https://github.com/datomatic/laravel-enum-helper/tree/main/tests)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/datomatic/laravel-enum-helper/run-tests?label=tests&color=5FE8B3&style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAcCAMAAABF0y+mAAABiVBMVEUAAAD/iPv9yP3Xm+j/mP//wfVj67Je6bP/h/pVx6p6175d57WQycf+iPn/iPrsnezArd3+t/qpvNJd6LP/jPpu6rv/lPr/kPpc57T/rvtc57Np6rj3oPl37cL/tfn/wv9d6brX//L/g/rYn+n/gvrWm+di6LX+jPrskfGWzMpt6bln4bdd57Jk6LWSycj+vPquwNVo6rde6bP7nvvYnup91b/+vfv/lvtc57OqvNTFs9//t/td57L9t/r/iPpd6LPapej/ovp26bxy67v9lfld6LJr4Ljwsvb/xv3/jv39zv1t6buG5cTDreH5ivlc5rJy676V4cxb57D/y/h50MOy4OCUxcVa77X/iPpe6LP/jP+pu9L8t///tvuQycfArNxp6LzArd151r7/i/9n4bb/j/9e6rT/ifr7ifrskvLYnuhi87tg8blg7bf/vv//lP+wxNtj9b3/qv//oP/+ivz/l/r8ifryn/fvlPTfpPDeofDKtujHtOWX1NF/4seC3cR82sFu7cBo5LiMwPMrAAAAWHRSTlMA/Wv8FAIC/dME/Wj+3tEG/Pv798G1oHRjS0k1LBsWDgsJ/v36+fTy8ezn4+Lh29XNzMzLysLAwLSwr66opJqakY+Ni4J7end0bGlpY11XU048KicmIR8fizl+vwAAAVdJREFUKM9tz2VXAlEQgOFBBURpkE67u7u7E1YFYQl1SbvrlztDiLvss+fc/fCemXMvAEhhKqU759P1rLoxUDUyEh9fPH0z7ALiVrEY+SSNtxNS2upouYv7hOL191aKVsZHUTgbnQPQgDkq4ctHdoQmTWmW4WFzlVUDVpNKXf2fWpWbZIwUq/hcmjWGYnSa1pZZjEoomrEdVAisD7CX6GEb40rqTODxCj21OjDOvjRV8l2jhudBDchg/FUbDIZCITzwQyH6a9+2AMDbm9GfltFnxgAdtQWUgQJl4VQq37uPcSnsfYZzav6Ew18fQ4fUYPM7Qn4uSiIdyx5saJ6T+/3+5KSltshicwI2UpfAKE/aoARTvnn7KMYMdlAUyWRSyHN2JeU42HlCi4TszTHcmuj3iMVdP5JzoyAWNzi6T3ZGrMFCliK3BAqRSC/B2+6IxvYYNcO+2Npfv+yFi10LfBUAAAAASUVORK5CYII=)](https://github.com/datomatic/laravel-enum-helper/actions/workflows/run-tests.yml)
[![GitHub Code Style Action Status](https://img.shields.io/github/workflow/status/datomatic/laravel-enum-helper/Check%20&%20fix%20styling?label=code%20style&color=5FE8B3&style=for-the-badge)](https://github.com/datomatic/laravel-enum-helper/actions/workflows/php-cs-fixer.yml)
[![Total Downloads](https://img.shields.io/packagist/dt/datomatic/laravel-enum-helper.svg?style=for-the-badge)](https://packagist.org/packages/datomatic/laravel-enum-helper)

This is an extension of the [datomatic/enum-helper](https://github.com/datomatic/enum-helper) package based on Laravel Framework.
The package consists on a `LaravelEnum` trait that extends `EnumHelper` (`EnumInvokable`, `EnumFroms`, `EnumNames`,
`EnumValues`, `EnumEquality`) and add dynamic methods to return a translation or "property" method and
relative helper methods.

You can think about it as an [`EnumDescription` trait](https://github.com/datomatic/enum-helper#descriptions-and-translations) but completely dynamic.

So you can define a custom method and have these functions available: `[method]s()`, `[method]sByName()`,
`[method]sByValue()`, `[method]sAsSelect()`.

For example, you can define a `color()` method and obtain automatically `colors()`, `colorsByName()`, `colorsByValue()`,
`colorsAsSelect()` methods.

The cool thing is you can also avoid writing the method and write the translations.
For example, you can define the property `excerpt` by writing the translations on enum.php (see below for explanation)
and obtain `excerpt()`, `excerpts()`, `excerptsByName()`, `excerptsByValue()`, `excerptsAsSelect()` methods.

The package use the [Laravel `Pluralizer` component](https://laravel.com/docs/localization#pluralization-language) to get the singular method to call or to translate.

If you are using [Laravel Nova](https://nova.laravel.com/) you can see the [Laravel Nova Enum Field](#laravel-nova-enum-field)

## The `enum-helper` base package summary
You should see the `datomatic/enum-helper` details on his [repository](https://github.com/datomatic/enum-helper), this is a summary:
- **Invokable cases**: get the value of enum "invoking" it statically
- **Construct enum by name or value**: `from()`, `tryFrom()`, `fromName()`, `tryFromName()` for all enums
- **Enums Equality**:  `is()`, `isNot()`, `in()`, `notIn()` methods
- **Names**: methods to have a list of case names (`names()`, `namesByValue()`, `namesAsSelect()`)
- **Values**: methods to have a list of case values (`values()`, `valuesByName()`)
- **Unique ID**: get an unique identifier from instance or instance from identifier (`uniqueId()`, `fromUniqueId()`)
- **Descriptions & Translations**: add description to enum with optional translation (`description()`,`descriptions()`,`descriptionsByName()`,`descriptionsByValue()`,`descriptionsAsSelect()`)


## Installation

Laravel 8 or above and PHP 8.1+ are required.

```sh
composer require datomatic/laravel-enum-helper
```

## Usage

You can use this functionality simply using the `LaravelEnum` trait.

```php
use Datomatic\LaravelEnumHelper\LaravelEnum;

// Pure enum 
enum Status
{
    use LaravelEnum;

    case PENDING;
    case ACCEPTED;
    case DISCARDED;
    case NO_RESPONSE;

    public function color(): string
    {
        return match ($this) {
            self::PENDING => '#000000',
            self::ACCEPTED => '#0000FF',
            self::DISCARDED => '#FF0000',
            self::NO_RESPONSE => '#FFFFFF',
        };
    }
}

// BackedEnum
enum StatusString
{   
    use LaravelEnum;

    case PENDING = 'P';
    case ACCEPTED = 'A';
    case DISCARDED = 'D';
    case NO_RESPONSE = 'N';
    
    // or public function color(?string $lang = null): string
    public function color(): string
    {
        ...
    }
```
After that you can define a custom "property" method like `color()` or `color(?string $lang = null)` or define the translations instead.

## Translations

Using this trait there is 2 way to manage translation strings.

### Using Short Keys
Language strings may be stored in `enums.php` files within the `lang` directory. Within this directory, there may be subdirectories for each language supported by the application.
```
/lang
    /en
        enums.php
    /it
        enums.php
```
All language files return an array of keyed strings. The array has 2 levels: the first level has as a key the complete class name of the enum, and the second has as a key the name of the enum case.
```php
// /lang/it/enums.php

return [
    Status::class => [
        'description' => [ // or property do you want to translate
            'PENDING' => 'In attesa',
            'ACCEPTED' => 'Accettato',
            'DISCARDED' => 'Rifiutato',
            'NO_RESPONSE' => 'Nessuna Risposta',
        ]
    ],
     // or using the enum object name attribute
    StatusString::class => [
        'description' => [
            StatusString::PENDING->name => 'In attesa',
            StatusString::ACCEPTED->name => 'Accettato',
    ...
```

### Using Translation Strings As Keys
Language strings are stored as JSON files in the lang directory (e.g. `lang/it.json`).
In this example the `description` property is translated:
```json
{
  "enums.Namespace\\StatusString.description.PENDING": "In attesa",
  "...":"..."
}
```
But if you want to use this way, you can simply define the method on Enum class like this `description` method.

```php
public function description(?string $lang = null): string
{
    return match ($this) {
        self::PENDING => __('Await decision', $lang),
        self::ACCEPTED => __('Recognized valid', $lang),
        self::DISCARDED => __('No longer useful', $lang),
        self::NO_RESPONSE => __('No response', $lang),
    };
```

## `[property]()` method
This dynamic method try to resolve `property()` method on the enum.  
If the method not exist try to translate the instance value with the framework translation function 
`__("enums.Namespace\EnumClass.property.CASE_NAME")`.  
In case the translation not exist throw an `TranslationMissing` exception.


## static `[property]s()` method

This dynamic method gets a list of case `property()` returns of the enum.
The name of the method is the plural of the property so if you are using `property` it will be `properties()`. 

```php
StatusString::descriptions(); // ['Await decision','Recognized valid','No longer useful','No response']
StatusString::colors(); // ['#000000','#0000FF','#FF0000','#FFFFFF']
// Subset
StatusString::descriptions([StatusString::ACCEPTED, StatusString::NO_RESPONSE]); // ['Recognized valid','No response']
StatusString::colors([StatusString::ACCEPTED, StatusString::NO_RESPONSE]); // ['#0000FF','#FFFFFF']
// Forcing language
Status::descriptions(null, 'it'); // 🇮🇹 ['In attesa','Accettato','Rifiutato','Nessuna Risposta']
StatusString::colors(null, 'it'); // ['#000000','#0000FF','#FF0000','#FFFFFF']
// Subset and language 
Status::descriptions([Status::NO_RESPONSE, Status::DISCARDED], 'it'); // 🇮🇹 ['Nessuna Risposta', 'Rifiutato']
StatusString::colors([StatusString::ACCEPTED, StatusString::NO_RESPONSE], 'it'); // ['#0000FF','#FFFFFF']
```

## static `[property]sByName()` method
This dynamic method returns an associative array of [case name => `property()` result].
The name of the method is the plural of the property so if you are using `property` it will be `propertiesByName()`.

```php
StatusString::descriptionsByName(); // ['PENDING' => 'Await decision', 'ACCEPTED' => 'Recognized valid',...
StatusString::colorsByName(); // ['PENDING' => '#000000','ACCEPTED' => '#0000FF',...
Status::descriptionsByName(); // ['PENDING' => 'Await decision', 'ACCEPTED' => 'Recognized valid',...
// Subset
StatusString::descriptionsByName([StatusString::DISCARDED, StatusString::ACCEPTED]); // ['DISCARDED' => 'No longer useful', 'ACCEPTED' => 'Recognized valid']
Status::descriptionsByName([[Status::PENDING, Status::DISCARDED]); // ['PENDING' => 'Await decision', 'DISCARDED' => 'No longer useful']
// Forcing language
StatusString::descriptionsByName(null, 'it'); // 🇮🇹 ['P' => 'In attesa','A' => 'Accettato',...
// Subset and language 
Status::descriptionsByName([Status::DISCARDED, Status::NO_RESPONSE], 'it'); // 🇮🇹 ['DISCARDED' => 'Rifiutato','NO_RESPONSE' => 'Nessuna Risposta',...
```

## static `[property]sByValue()` method
This dynamic method returns an associative array of [case value => `property()` result]  on `BackedEnum`, throw `NotBackedEnum` exception otherwise.
The name of the method is the plural of the property so if you are using `property` it will be `propertiesByValue()`.

```php
StatusString::descriptionsByValue(); // ['P' => 'Await decision', 'A' => 'Recognized valid',...
StatusString::colorsByValue(); // ['P' => '#000000','A' => '#0000FF',...
Status::descriptionsByValue(); // throw `NotBackedEnum` exception
// Subset
StatusString::descriptionsByValue([StatusString::DISCARDED, StatusString::ACCEPTED]); // ['D' => 'No longer useful', 'A' => 'Recognized valid']
StatusString::colorsByValue([[Status::PENDING, Status::DISCARDED]); // ['P' => '#000000', 'D' => '#FF0000']
// Forcing language
StatusString::descriptionsByValue(null, 'it'); // 🇮🇹 ['P' => 'In attesa','A' => 'Accettato',...
// Subset and language 
StatusString::descriptionsByValue([StatusString::DISCARDED, StatusString::NO_RESPONSE], 'it'); // 🇮🇹 ['D' => 'Rifiutato','N' => 'Nessuna Risposta',...
```

## static `[property]sAsSelect()` method
This dynamic method returns an associative array of [case value => `property()` result]  on `BackedEnum`,  [case name => `property()` result] otherwise.
The name of the method is the plural of the property so if you are using `property` it will be `propertiesAsSelect()`.

```php
StatusString::descriptionsAsSelect(); // ['P' => 'Await decision', 'A' => 'Recognized valid',...
StatusString::colorsAsSelect(); // ['P' => '#000000','A' => '#0000FF',...
Status::descriptionsAsSelect(); // ['PENDING' => 'Await decision', 'ACCEPTED' => 'Recognized valid',...
// Subset
Status::descriptionsAsSelect([Status::PENDING, Status::DISCARDED]); // ['PENDING' => 'Await decision', 'DISCARDED' => 'No longer useful']
StatusString::colorsAsSelect([StatusString::PENDING, StatusString::DISCARDED]); // ['P' => '#000000', 'D' => '#FF0000']
// Forcing language
StatusString::descriptionsAsSelect(null, 'it'); // 🇮🇹 ['P' => 'In attesa','A' => 'Accettato',...
Status::descriptionsAsSelect(null, 'it'); // 🇮🇹 ['PENDING' => 'In attesa', 'ACCEPTED' => 'Accettato',...
// Subset and language 
Status::descriptionsAsSelect([Status::DISCARDED, Status::NO_RESPONSE], 'it'); // 🇮🇹 ['DISCARDED' => 'Rifiutato','NO_RESPONSE' => 'Nessuna Risposta',...
```

## Laravel Nova Enum Field
If you are using [Laravel Nova](https://nova.laravel.com/) Administrator Panel you can use a package to support the `enum-helper` or/and `laravel-enum-helper`.  
This package adds the PHP 8.1 `enum`, `EnumDescription` and `LaravelEnum` traits support to Nova, with a Nova Select and Nova Boolean filters ready out of the box.

Package: [datomatic/nova-enum-field](https://github.com/datomatic/nova-enum-field)