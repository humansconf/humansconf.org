# humansconf.org
source for humansconf.org

## How to add yourself to the list of organizers

If you want to use your gravatar image, generate the md5 hash of your email address like this:

```sh
echo hello@example.org | ruby -r digest/md5 -n -e 'p Digest::MD5.hexdigest($_.downcase.strip)'
```

Otherwise, add your photo to `images/organizers`.

Add your name and either your gravatar digest or the path to your image to the `_data/organizers.yml`.
