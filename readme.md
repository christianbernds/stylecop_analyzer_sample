# StyleCop Analyzer Sample

StyleCop Analyzer Sample ist ein .NET Core Projekt zur Sicherstellung von Codequalität mittels StyleCop Regeln.


## Was sind die Ziele dieses Projekts?

Ich möchte hiermit aufzeigen wie die StyleCop Analyzer in ein .NET Core Projekt eingebunden und verwendet werden können. Dabei wurden einige StyleCop Regeln aktiviert/deaktiviert bzw. konfiguriert.


## Relevante URLs

* [StyleCop.Analayzers mit DotNet-CLI](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/DotNetCli.md)
* [Known Changes zwischen StyleCop.Analyzers und StyleCop Classic](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/KnownChanges.md)
* [Konfiguration des StyleCop.Analyzers](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/Configuration.md)
* [Regeln: Documentation](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/DocumentationRules.md)
* [Regeln: Layout](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/LayoutRules.md)
* [Regeln: Maintainability](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/MaintainabilityRules.md)
* [Regeln: Naming](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/NamingRules.md)
* [Regeln: Ordering](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/OrderingRules.md)
* [Regeln: Readability](https://github.com/DotNetAnalyzers/StyleCopAnalyzers/blob/master/documentation/ReadabilityRules.md)


## Wie kann ich das Projekt aufsetzen?


### Voraussetzungen

* .NET Core `>= 2.0.0`


### Setup/Installation

```shell
$ cd StyleCopTest
$ dotnet restore
$ dotnet build
```

## Wie kann ich das Projekt benutzen?

Durch den `dotnet build` Vorgang wird in der Konsole jeder StyleCop verstoß als Warnung protokolliert.

```shell
$ dotnet build
```


## Was muss ich sonst noch wissen?

* Regeln können innerhalb des `stylecop.ruleset` aktiviert/deaktiviert werden
* Für verschiedene Regeln können weitere Einstellungen getätigt werden, diese werden in der `stylecop.json` vorgenommen


## Offene Punkte

* stylecop.json und stylecop.ruleset anpassen
* `Missing XML comment for publicly visible type or member 'Class1' [StyleCopTest]` beheben, da <NoWarn> innerhalb der `.csproj`-Datei nicht eingreift um diesen Fehler aus dem Problem-Tab von VSCode zu löschen.



### Wen kann ich auf das Projekt ansprechen?

* Christian Bernds
