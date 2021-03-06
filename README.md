# Hexo-Prism-Plugin

Since `highlight.js` didn't support JSX syntax properly, I wrote this plugin to replace
Hexo's default code highlight plugin.

## Install
```
npm i -S hexo-prism-plugin
```
## Usage
First, you should edit your `_config.yml` by adding following configuration.

```yaml
prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'default'
  line_number: false    # default false
```
Note: check `_config.yml` `highlight` option. Make sure that
```yaml
highlight:
  enable: false
```

- `mode`:
  - realtime  (Parse code on browser in real time)
  - preprocess  (Preprocess code in node)

- `theme`:
  - default
  - coy
  - dark
  - funky
  - okaidia
  - solarizedlight
  - tomorrow
  - twilight

- `line_number`:
  - true (Show line numbers)
  - false (Default, Hide line numbers)

And then, clean and generate project by running command:

```
hexo clean
```

```
hexo g
```

Note: if you change theme, you should re-generate your project.

## License
MIT
