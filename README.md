# The Courseware Quiz Builder

The jQuery quiz builder I wrote for The Coursewa.re Project.

[![Build Status](https://travis-ci.org/Courseware/quiz-builder.png?branch=master)](https://travis-ci.org/Courseware/quiz-builder)

## Installation

Download the latest file from `src` directory.

## Usage
This plugin uses HTML5 storage for questions instead of HTML tag.
The purpose of this fork is to instantiate plugin in event listener(ex: `click element`). The plugin is used especially with [Meteor.js](https://meteor.com) projects.

For usage and examples check the `index.html` file.
To instantiate plugin add this into your `.html` file or to an event listener.
```javascript
$('[data-quiz="auto"]').each(function () {
  var $quiz = $(this);
  $quiz.quizBuilder($quiz.data());
})
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Run and update the tests. See below how.
5. Push to the branch (`git push origin my-new-feature`)
6. Create new Pull Request

## Tests

Check `spec` directory for Jasmine tests.

To run those, open `spec/runner.html` in a browser or use `Rake`

```bash
$ bundle update
$ bundle exec rake
```

## Credits

This library was extracted from the [http://coursewa.re](Coursewa.re) project.

## License

MIT.
