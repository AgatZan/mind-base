

### Примеры

	tool/_paragraph-spacing.scss
```scss
@mixin paragraphSpacing() {
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