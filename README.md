# Digital Rain

Digital Rain is an HTML5 + Canvas demo app written entirely in [Go](https://go.dev/).
It's intended to mimic the look of the [falling text](https://www.youtube.com/watch?v=rpWrtXyEAN0) in the movie [The Matrix](https://www.imdb.com/title/tt0133093/).

[Live Demo](https://matrix.yesmar.com/)

## Notes on the fork

* Instructions updated to use the latest version of GopherJS
* Fixed links to point to the right places using https
* Removed github.com link overlay and commented out the click event handler for a cleaner presetation
* Changed hard coded page title to a variable and updated the message

## Build

Install [Go](https://go.dev/dl) and [GopherJS](https://github.com/gopherjs/gopherjs)

```bash
go install golang.org/dl/go1.19.13@latest
go1.19.13 download
export GOPHERJS_GOROOT="$(go1.19.13 env GOROOT)"
go1.19.13 install github.com/gopherjs/gopherjs@v1.19.0-beta1
gopherjs build digitalrain.go --minify
gopherjs serve
```

## License

Digital Rain is available under the [MIT License](LICENSE).
