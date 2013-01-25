jscompile
=========
Helper bash script to compile/compress JavaScript sources.

This is a simple front-end wrapper that calls Closure Compiler, YUI
Compressor, UglifyJS, or cat. The main benefit is a unified command
line and ability to specify multiple input source files.

    usage: jscompile [options] infile [infile2 ...]
    
    options:
        --output file    -o file    Set output file name [default stdout]
        --closure        -c         use Closure compiler [default]
        --yuicompressor  -y         use YUICompressor
        --uglifyjs       -u         use UglifyJS
        --cat            -t         just concatenate
    
    environment:
        JSCOMPILE_COMPILER name     set default compiler (closure,
                                    yuicompressor, uglifyjs, cat)
