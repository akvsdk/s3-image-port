# S3 Image Port

A custom frontend panel created to manage images hosted on S3-like (Cloudflare R2, for example) storage services, where traditionally no specialized image management panel exists. This solution brings a simple yet powerful user interface to handle image uploads, management, and integration within your projects.

## Live Instance

A public instance is hosted on Vercel and can be accessed at [iport.yfi.moe](https://iport.yfi.moe). You can start using it immediately by entering your specific S3 settings under the Settings tab. While the source code is open and guarantees no server-side data processing (ensuring your privacy and security), you have the option to fork the repository and deploy it on your own Vercel account or server.

## Features

- **Upload Photos:** Upload images with options to convert formats before uploading.
- **Display Image List:** View a gallery of all uploaded images.
- **Copy Image Links:** Easily copy direct and markdown formatted image links.
- **Delete Images:** Remove images from storage directly through the panel.

The interface is fully responsive and works seamlessly on mobile devices as well.

## Usage Instructions

Before using the application, configure your S3 settings in the Settings tab. Required fields include the S3 endpoint, bucket name, region, and two keys (access key and secret key). Optional advanced settings like setting a public URL format are available if your S3 bucket uses a custom domain.

For obtaining S3 related keys, please refer to the documentation of your storage service provider. For instance, for R2 buckets managed under Cloudflare, keys are available under the "Manage API Tokens" section. Note that you will need the "Access Key ID" and "Secret Access Key", not the "Token Value" provided by Cloudflare.

## Feedback and Contributions

Feel free to raise an issue if you encounter any problems or have suggestions.
If you have ideas for new features, don’t hesitate to create an issue for those as well—no idea is too far-fetched!

## Known Issues / Roadmap

- [ ] Customize upload key
- [ ] Image preview before upload
- [ ] Not able to fetch all image if there are more than 1000 objects in the bucket
- [ ] Distinguish image files from other files
