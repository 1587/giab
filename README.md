# giab
a tool for "giab" (github issue as blog) guys

## Install

```bash
npm install giab
```

## Usage

1) Go to your repository's root dir

2) Make sure you have a readme file named **README.md**

3) Add placeholder to **README.md**, like this:

```html
<!--giab:issue_list_start-->
your articles will be shown here
<!--giab:issue_list_end-->
```

4) Add a config file named **.giabrc**, sample content:

```javascript
{
  "type": "basic",
  "username": "simongfxu",
  "password": "password here",
  "issues": {
    "repo": "simongfxu.github.com",
    "owner": "simongfxu"
  }
}
```

5) Edit .gitignore file in your repository's root dir, add a line

```html
.giabrc
```

NOTE: this is very important, I do not think you will let everybody know your password.

6) Execute the following command

```bash
node node_modules/giab
```

That is all!

[See an example](https://github.com/simongfxu/simongfxu.github.com)