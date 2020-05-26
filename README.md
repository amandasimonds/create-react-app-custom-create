create-react-app my-app --scripts-version 1.1.5

npm run eject

web config files:

1st one: around 167 under 

            test: /\.css$/,
            use: [
              require.resolve('style-loader'),
              {
                loader: require.resolve('css-loader'),
                options: {
                  importLoaders: 1,
                  modules: true,
                  localIdentName: "[name]__[local]__[hash:base64:5]"
                },
              },

modules: true,
localIdentName: "[name]__[local]__[hash:base64:5]"

2nd one: around 186

                 use: [
                    {
                      loader: require.resolve('css-loader'),
                      options: {
                        importLoaders: 1,
                        minimize: true,
                        sourceMap: shouldUseSourceMap,
                        modules: true,
                        localIdentName: "[name]__[local]__[hash:base64:5]"
                      },


modules: true,
localIdentName: "[name]__[local]__[hash:base64:5]"


