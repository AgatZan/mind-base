

### Примеры

	tool/_paragraph-spacing.scss
```scss
@mixin paragraphSpacing($paragraph-spaces) {
    margin-top: 0;

    @include mediaEachMax((
        margin-bottom: $paragraph-spaces,
    ));

    * + & {
        @include mediaEachMax((
            margin-top: $paragraph-spaces,
        ));
    }

    &:last-child {
        margin-bottom: 0;
    }
}
```

	tool/_fibbonachi.scss
```scss
@function fibonacci($n) {
  $sequence: 0 1;
  @for $_ from 1 through $n {
    $new: nth($sequence, length($sequence)) + nth($sequence, length($sequence) - 1);
    $sequence: append($sequence, $new);
  }
  @return nth($sequence, length($sequence));
}
```