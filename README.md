# lein-bom

A Leiningen plugin that provides support for importing Maven "Bill Of Materials" (BOM) dependencies.

```clojure
[helpshift/lein-bom "0.2.0"]
```

## Install

Put `[lein-bom "0.2.0"]` into the `:plugins` vector of your `project.clj`.

## Usage

Specify bom dependencies using `:import` vector in `:bom` map of your `project.clj`.

```clojure
:bom {:import [[com.fasterxml.jackson/jackson-bom "2.9.3"]]}
```

To see actual managed dependencies, run:

```
$ lein bom
```

## License

Distributed under the [Eclipse Public License](http://www.eclipse.org/legal/epl-v10.html).
