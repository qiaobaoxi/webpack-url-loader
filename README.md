# webpack-url-loader
` module.exports = {
  module: {
    rules: [
      {
        test: /\.(png|jpg|gif)$/,
        use: [
          {
            loader: 'url-loader',
            options: {
              limit: 8192
            }
          }
        ]
      }
    ]
  }
}`
### name	type	default	description
### limit	{Number}	undefined	Byte limit to inline files as Data URL
### mimetype	{String}	extname	Specify MIME type for the file (Otherwise it's inferred from the file extension)
### fallback	{String}	file-loader	Specify loader for the file when file is greater than the limit (in bytes)

图片的压缩
