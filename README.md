# NAME

Color::Brewer - Color schemes from Cynthis Brewer's ColorBrewer [http://colorbrewer2.org/](http://colorbrewer2.org/)

# SYNOPSYS

        use Color::Brewer;

        my @color_scheme = Color::Brewer::named_color_scheme(name => 'RdBu', number_of_data_classes => 4);
        my @color_schemes = Color::Brewer::color_schemes(data_nature => 'sequential', number_of_data_classes => 5);

# DESCRIPTION

Provides color schemes for maps designed by Cynthia Brewer. The color schemes are also suitable for data visualizations.

Choosing the best color scheme is easy. Just visit Cynthia Brewer's ColorBrewer [http://colorbrewer2.org](http://colorbrewer2.org).

# METHODS

## named\_color\_scheme

Get a named color scheme

### Parameters

- name:

    Name of the color scheme: RdBu

- number\_of\_data\_classes:

    Number of data classes. Valid range goes from 3 to 12 depending on the scheme.

### Returns

Array with the color scheme or an empty list if there is no such scheme

## color\_schemes

Get the color schemes available

### Parameters

- data\_nature: 

    Nature of the data: qualitative, sequential or diverging

- number\_of\_data\_classes:

    Number of data classes. Valid range goes from 3 to 12 depending on the scheme.

### Returns

Array with all the color schemes matching the options. Every color scheme is an array 
which elements are html rgb colors like: "rgb(252,141,89)"

Array can be empty if none of the color schemes match the options.

# CREDIT

Color Brewer website and color schemes are copyrighted by Cynthia Brewer. With this module is bundled a json file with the color schemes. 

This product includes color specifications and designs developed by Cynthia Brewer (http://colorbrewer2.org/).

        Apache-Style Software License for ColorBrewer software and ColorBrewer Color Schemes

        Copyright (c) 2002 Cynthia Brewer, Mark Harrower, and The Pennsylvania State University.

        Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.
        You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

        Unless required by applicable law or agreed to in writing, software distributed
        under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
        CONDITIONS OF ANY KIND, either express or implied. See the License for the
        specific language governing permissions and limitations under the License.

# SEE ALSO

[Color::Scheme](https://metacpan.org/pod/Color::Scheme) Perl implementation of Color Schemes 2 

[Color::Palette](https://metacpan.org/pod/Color::Palette) Set of named colors

[Color::Library](https://metacpan.org/pod/Color::Library) Named-color library

[Graphics::Color](https://metacpan.org/pod/Graphics::Color) Simple creation and manipulation of colors

[Graphics::ColorObject](https://metacpan.org/pod/Graphics::ColorObject) Conversion between color spaces

# AUTHOR

Pablo Rodríguez González

# LICENSE

This work is licensed under the Apache License, Version 2.0.
