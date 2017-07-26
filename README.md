Tämä sivusto buildataan
[Middlemanillä](https://middlemanapp.com/),
eli:

	sudo apt install npm nodejs nodejs-legacy
	gem install middleman
	npm install babel-core babel-loader babel-preset-es2015 css-loader extract-text-webpack-plugin gulp gulp-plumber node-sass postcss-loader sass-loader webpack webpack-stream babel-polyfill bootstrap bowser lodash store visibilityjs
	bundle exec middleman build

Buildatut tiedostot näkyvät `build/`-hakemistossa. Kopioi ne
[opiskelija-dashboard.github.io-repositorioon](https://github.com/opiskelija-dashboard/opiskelija-dashboard.github.io)
jollakin menetelmällä, vaikka drag-n-dropilla tai minun suosimalla tervapallomenetelmällä, joka on aika turvallinen hakemistopuiden säilyttämisen suhteen:

	cd build/
	tar -cvf buildi.tar ./*
	mv buildi.tar ../../opiskelija-dashboard.github.io/
	cd ../../opiskelija-dashboard.github.io/
	tar -xvf buildi.tar
	rm buildi.tar

