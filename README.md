### A clone of React Boilerplate Project integrated with Structor (former React UI Builder).
***The clone is synced with every React Boilerplate release***

React Boilerplate is a highly scalable, offline-first foundation with the best DX and a focus on performance and best practices.

React Boilerplate lets you start your next react project in seconds.

Learn more in <a href="https://github.com/mxstbr/react-boilerplate">React Boilerplate repo</a>

> Please note that this boilerplate is **production-ready and not meant for beginners**! If you're just starting out with react or redux, please refer to https://github.com/petehunt/react-howto instead. If you want a solid, battle-tested base to build your next product upon and have some experience with react, this is the perfect start for you.

This clone lets you use Structor in application which was bootstrapped with React Boilerplate. 

Generate the source code for components, containers, routes, selectors and sagas in Structor using sophisticated generators. 

Additionally, search full-fledged React components on [Structor Market](https://helmetrex.com) and install them right into the app.
 
Learn more in <a href="https://github.com/ipselon/structor">Structor ReadMe</a>

#### Getting started

1. Clone this repo using `git clone https://github.com/ipselon/react-boilerplate-clone.git` OR download and unpack ZIP [master.zip](https://github.com/ipselon/react-boilerplate-clone/archive/master.zip).
1. Run `npm run setup` to install dependencies and clean the git repo.
1. At this point you can run `npm start` to see the example app at `http://localhost:3000`.
1. Run `npm run clean` to delete the example app.

#### Running Structor

1. Run `npm run structor`
1. Open in the browser Structor's workspace: `http://localhost:2222/structor`.

Now you're ready to rumble!

#### The changes made in original boilerplate

1. `.structor` metadata directory is added.
1. Additional `structor` command is added into `scripts` section in `package.json` file.
1. Additional `app/assets` directory is added.
1. In order to use custom CSS files without packing them into npm modules the following changes were made in `webpack.base.babel.js`:
```diff
{
  test: /\.css$/,
-  include: /node_modules/,
+  include: [/node_modules/, /app[\\\/]assets/],
  loaders: ['style-loader', 'css-loader'],
}
``` 

## License

This project is licensed under the MIT license, Copyright (c) 2016 Maximilian
Stoiber. For more information see [LICENSE.md](https://github.com/mxstbr/react-boilerplate/blob/master/LICENSE.md).
