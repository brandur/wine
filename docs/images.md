# Image documentation

Install Image Magick via Homebrew:

    brew install imagemagick

Use these commands for image resize:

    export GMI=<image path>
    export GMO=tasting-notes/2019

    magick convert $GMI -resize 1100x733^ -gravity center -extent 1100x733 -quality 85 $GMO/${$(basename $GMI)/.jpg/@2x.jpg}
