# Vendor-Prefixes
A collection of vendor prefixes designed to enhance cross-browser compatibility, ensuring your projects are accessible to all users, including those on older browsers.

## Features
1. **Comprehensive Prefix Support**: Contains a wide array of vendor prefixes, ensuring compatibility across various browsers.
2. **Regular Updates**: This repository is regularly updated to include new prefixes and maintain compatibility.

## Integration
1. 

## Usage
1. Create a scss file in which you want to add the vendor prefixes
2. Use an @use statement like this:
@use "./vendor-prefix" as prefix
3. Now if you want to use a prefix you just have to write prefix.\[property\], with property changing depending on what you want
### Example usage
```
@use "./vendor-prefix" as prefix;
.box {
  @include prefix.animation(rotate 4s);
  width: 5rem;
  height: 5rem;
}
```
Compiles to:
```
.box {
  -webkit-animation: rotate 4s;
  -o-animation: rotate 4s;
  -moz-animation: rotate 4s;
  animation: rotate 4s;
  width: 5rem;
  height: 5rem;
}
```
## Roadmap
This project will continue to be maintained. Upcoming updates will include:

1. Expansion of the prefix list to encompass all vendor prefixes from older browsers, ensuring 100% accessibility.

## Report a Bug & Reach Me
Encountered an issue or have suggestions? Please [create an issue](https://github.com/tomScheers/vendor-prefixes/issues) on GitHub. Interested in collaboration or have questions? Reach out [here](https://github.com/tomScheers)!
