# Comparing `tmp/jaraco.site-6.7.0.tar.gz` & `tmp/jaraco.site-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.site-6.7.0.tar", last modified: Sun Mar 31 08:35:12 2024, max compression
+gzip compressed data, was "jaraco.site-6.8.0.tar", last modified: Tue Apr  2 22:46:51 2024, max compression
```

## Comparing `jaraco.site-6.7.0.tar` & `jaraco.site-6.8.0.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.651027 jaraco.site-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.599027 jaraco.site-6.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.599027 jaraco.site-6.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-31 08:35:12.651027 jaraco.site-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/Procfile
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.599027 jaraco.site-6.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/fabfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.591027 jaraco.site-6.7.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.603027 jaraco.site-6.7.0/jaraco/site/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/landing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/openid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.603027 jaraco.site-6.7.0/jaraco/site/projecthoneypot/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/projecthoneypot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29425 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/projecthoneypot/croakysteel.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/resume.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.591027 jaraco.site-6.7.0/jaraco/site/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.603027 jaraco.site-6.7.0/jaraco/site/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.603027 jaraco.site-6.7.0/jaraco/site/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/blog.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/fosstodon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/info.png
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/keybase.svg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/linkedin.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25753 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/ok.png
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/stackoverflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/images/twitter.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.603027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/blueorange.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/compact.css
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/cssClasses.sh
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/cssClasses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/gray.css
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/original.css
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/professional.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/authors/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)   101285 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/copying/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/install/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/install/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.607027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.635027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-0.gif
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-1.gif
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-l.gif
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-r.gif
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-t.gif
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-u.gif
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html
--rw-r--r--   0 runner    (1001) docker     (127)    26387 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html
--rw-r--r--   0 runner    (1001) docker     (127)    15177 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css
--rw-r--r--   0 runner    (1001) docker     (127)   410745 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html
--rw-r--r--   0 runner    (1001) docker     (127)   172000 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.635027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/news/
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/news/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.635027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/todo/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.635027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/catalog
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.639027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.639027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/README
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/build.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/example1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/example2.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.639027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/java/
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.639027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.639027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.643027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/
--rw-r--r--   0 runner    (1001) docker     (127)    36336 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    31697 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    37763 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.643027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.643027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.647027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.647027 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/paper/
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.647027 jaraco.site-6.7.0/jaraco/site/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/chart example.html
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/master.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.647027 jaraco.site-6.7.0/jaraco/site/templates/openid/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/openid/about.html
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/openid/id.html
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/openid/yadis.html
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/templates/welcome.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.651027 jaraco.site-6.7.0/jaraco/site/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/ubuntu/jaraco.site.service
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/jaraco/site/ubuntu/nginx config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:35:12.651027 jaraco.site-6.7.0/jaraco.site.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-31 08:35:12.000000 jaraco.site-6.7.0/jaraco.site.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-03-31 08:35:12.000000 jaraco.site-6.7.0/jaraco.site.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 08:35:12.000000 jaraco.site-6.7.0/jaraco.site.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-31 08:35:12.000000 jaraco.site-6.7.0/jaraco.site.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 08:35:12.000000 jaraco.site-6.7.0/jaraco.site.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-31 08:35:12.651027 jaraco.site-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 08:34:58.000000 jaraco.site-6.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.892105 jaraco.site-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.840105 jaraco.site-6.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.840105 jaraco.site-6.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-02 22:46:51.892105 jaraco.site-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/Procfile
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.840105 jaraco.site-6.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/fabfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.832105 jaraco.site-6.8.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.840105 jaraco.site-6.8.0/jaraco/site/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/landing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/openid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/projecthoneypot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/projecthoneypot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29425 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/projecthoneypot/croakysteel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/resume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.832105 jaraco.site-6.8.0/jaraco/site/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/blog.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/fosstodon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/keybase.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/linkedin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25753 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/ok.png
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/stackoverflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/images/twitter.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/blueorange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/compact.css
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/cssClasses.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/cssClasses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/gray.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/original.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/professional.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.844105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.848105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/authors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.848105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)   101285 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.848105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/copying/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.848105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/install/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.848105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.876105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-0.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/box-1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-l.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-r.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-t.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/caret-u.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26387 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15177 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css
+-rw-r--r--   0 runner    (1001) docker     (127)   410745 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html
+-rw-r--r--   0 runner    (1001) docker     (127)   172000 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.876105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/news/
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/news/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.876105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/todo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.876105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/catalog
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.876105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.880105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/build.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/example1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/example2.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.880105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/java/
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.880105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.880105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.884105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/
+-rw-r--r--   0 runner    (1001) docker     (127)    36336 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    31697 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    37763 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.884105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.884105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.888105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.888105 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.888105 jaraco.site-6.8.0/jaraco/site/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/chart example.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/master.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.888105 jaraco.site-6.8.0/jaraco/site/templates/openid/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/openid/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/openid/id.html
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/openid/yadis.html
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/templates/welcome.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.888105 jaraco.site-6.8.0/jaraco/site/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/ubuntu/jaraco.site.service
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/jaraco/site/ubuntu/nginx config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:46:51.892105 jaraco.site-6.8.0/jaraco.site.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-02 22:46:51.000000 jaraco.site-6.8.0/jaraco.site.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-04-02 22:46:51.000000 jaraco.site-6.8.0/jaraco.site.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:46:51.000000 jaraco.site-6.8.0/jaraco.site.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-02 22:46:51.000000 jaraco.site-6.8.0/jaraco.site.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 22:46:51.000000 jaraco.site-6.8.0/jaraco.site.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 22:46:51.892105 jaraco.site-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 22:46:35.000000 jaraco.site-6.8.0/tox.ini
```

### Comparing `jaraco.site-6.7.0/.github/workflows/main.yml` & `jaraco.site-6.8.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -44,21 +44,14 @@
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: "3.11"
           platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
-        exclude:
-        # lxml fails to build on Windows
-        # https://bugs.launchpad.net/lxml/+bug/1977998
-        - platform: windows-latest
-          python: "3.11"
-        # lxml fails to build on Python 3.12
-        - python: "3.12"
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `jaraco.site-6.7.0/LICENSE` & `jaraco.site-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/PKG-INFO` & `jaraco.site-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.site
-Version: 6.7.0
+Version: 6.8.0
 Summary: jaraco.com main website
 Home-page: https://github.com/jaraco/jaraco.site
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.site-6.7.0/README.rst` & `jaraco.site-6.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/docs/conf.py` & `jaraco.site-6.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/fabfile.py` & `jaraco.site-6.8.0/fabfile.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/__init__.py` & `jaraco.site-6.8.0/jaraco/site/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/charts.py` & `jaraco.site-6.8.0/jaraco/site/charts.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/controllers.py` & `jaraco.site-6.8.0/jaraco/site/controllers.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,20 @@
         return "IPv6 confirmed"
 
     @cherrypy.expose
     def allurbase(self):
         return str(cherrypy.request.base)
 
     @cherrypy.expose(alias='résumé')
-    def resume(self, url=None):
-        return resume.Renderer(url).html()
+    def resume(self, url=None, emphasis=None):
+        return resume.Renderer(url=url, emphasis=emphasis).html()
 
     @cherrypy.expose(alias='résumé.pdf')
-    def resume_pdf(self, url=None):
-        res = resume.Renderer(url).pdf()
+    def resume_pdf(self, url=None, emphasis=None):
+        res = resume.Renderer(url=url, emphsis=emphasis).pdf()
         # only set the content type if the rendering succeeded
         cherrypy.response.headers['Content-Type'] = 'application/pdf'
         return res
 
     @cherrypy.expose
     def auth(self):
         return "You authenticated as %s" % cherrypy.request.login
```

### Comparing `jaraco.site-6.7.0/jaraco/site/landing.py` & `jaraco.site-6.8.0/jaraco/site/landing.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/openid.py` & `jaraco.site-6.8.0/jaraco/site/openid.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/projecthoneypot/__init__.py` & `jaraco.site-6.8.0/jaraco/site/projecthoneypot/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/projecthoneypot/croakysteel.py` & `jaraco.site-6.8.0/jaraco/site/projecthoneypot/croakysteel.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/projects.py` & `jaraco.site-6.8.0/jaraco/site/projects.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/resume.py` & `jaraco.site-6.8.0/jaraco/site/resume.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import os
 import subprocess
 
 from requests_toolbelt import sessions
 from lxml import etree
 
 
+lookup = dict(
+    default='/s/sg48j6iuoc819jm/Jason%20R.%20Coombs%20resume.xml?dl=1',
+    packaging='/scl/fi/l2xop7gqgz30krxrmx2dw/Jason-R.-Coombs-resume-packaging.xml?rlkey=tm81tcbycqrz6t22t29w92l8j&dl=1',
+)
+
+
 class Renderer:
-    session = sessions.BaseUrlSession('https://dl.dropboxusercontent.com')
-    url = '/s/sg48j6iuoc819jm/Jason R. Coombs resume.xml'
+    session = sessions.BaseUrlSession('https://www.dropbox.com')
 
-    def __init__(self, url=None):
+    def __init__(self, url=None, emphasis=None):
+        self.url = lookup[emphasis or 'default']
+        print(self.url)
         if url:
             self.url = url
 
     def get_transform_path(self, output_name):
         path_tmpl = 'resume-1.5.1/xsl/output/{output_name}.xsl'
         path = path_tmpl.format(**locals())
         here = os.path.dirname(__file__)
         return os.path.join(here, 'static', path)
 
     def html(self):
         transform_path = self.get_transform_path('us-html')
         transform = etree.XSLT(etree.parse(open(transform_path)))
+        print(self.url)
         resp = self.session.get(self.url)
+        print(resp.content)
         src = etree.fromstring(resp.content)
         return str(transform(src))
 
     def pdf(self):
         "use subprocess and fop to render the output"
         cmd = ['fop', '-xml', '-', '-xsl', self.get_transform_path('us-letter'), '-']
         resp = self.session.get(self.url)
```

### Comparing `jaraco.site-6.7.0/jaraco/site/run.py` & `jaraco.site-6.8.0/jaraco/site/run.py`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/css/style.css` & `jaraco.site-6.8.0/jaraco/site/static/css/style.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/blog.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/blog.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/fosstodon.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/fosstodon.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/github.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/github.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/info.png` & `jaraco.site-6.8.0/jaraco/site/static/images/info.png`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/keybase.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/keybase.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/linkedin.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/linkedin.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/ok.png` & `jaraco.site-6.8.0/jaraco/site/static/images/ok.png`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/stackoverflow.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/stackoverflow.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/images/twitter.svg` & `jaraco.site-6.8.0/jaraco/site/static/images/twitter.svg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/NOTICE` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/NOTICE`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/blueorange.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/blueorange.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/compact.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/compact.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/gray.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/gray.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/original.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/original.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/css/professional.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/css/professional.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/authors/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/changelog/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/copying/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/install/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/install/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/appendixes.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/cssref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.academics.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievement.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.achievements.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.address.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.annotation.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.artTitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.author.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.award.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.awards.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.birth.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.bookTitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.break.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.citation.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.city.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearance.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.clearances.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.company.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.contact.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.copyright.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.country.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.county.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.date.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.dayOfMonth.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degree.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.degrees.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.description.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.docpath.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.email.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.emphasis.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.employer.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.fax.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.firstname.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.from.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.gpa.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.head.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.header.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.history.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.instantMessage.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.institution.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interest.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.interests.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.job.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.jobtitle.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keyword.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.keywords.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.label.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.lastModified.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.legalnotice.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.level.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.link.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.location.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.major.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.membership.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.memberships.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.middlenames.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.minor.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.misc.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.month.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.name.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.node.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.note.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.objective.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.organization.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pageNums.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pager.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.para.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.period.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.phone.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.possible.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.postalCode.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.prefecture.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.present.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.project.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.projects.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.province.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pub.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubDate.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.publisher.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.pubs.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referee.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.referees.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.result.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resume.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.resumes.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.score.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skill.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillarea.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillareas.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skills.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.skillset.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.state.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.street2.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subject.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.subjects.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suburb.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.suffix.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.surname.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.tail.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.title.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.to.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.uri.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.url.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.ward.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.year.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/element.zip.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/elementref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.about.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.create.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.features.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.explore.next-steps.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.install.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/getting-started.setup.software.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-1.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-10.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-11.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-2.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-3.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-4.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-5.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-6.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-7.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-8.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl-9.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gfdl.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/gloss.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/intro.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/manual.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.address.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.css.href.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.header.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.interest.description.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.referees.display.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.skills.level.display.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/param.subjects.format.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/paramref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/html/ref.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.css`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/manual/manual.txt`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/news/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/news/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/doc/todo/index.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/catalog` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/catalog`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/iso-lat1.ent`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/resume.dcl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/dtd/resume.dtd`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/Makefile` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/Makefile`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/Makefile`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/brazil.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/canada.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/ireland.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/italy.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/norway.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/nz.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/uk.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/untagged.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/addressing/usa.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/build.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/build.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/example1.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/example1.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/examples/example2.xml` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/examples/example2.xml`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/java/xmlresume-filter.jar`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/br.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/de.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/es.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/fr.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/it.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/nl.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/propogate-params.sh`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/uk.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/country/us.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/fo.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/format/text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/address.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/common.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/deprecated.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/pub.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/string.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/lib/textlayout.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/124-130.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/13x-140.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/default.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_contemporary.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/html_professional.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/misc/normalize-whitespace.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/br-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/de-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/fr-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/it-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/nl-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/uk-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-html.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-letter.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/output/us-text.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/paper/a4.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/paper/letter.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl` & `jaraco.site-6.8.0/jaraco/site/static/resume-1.5.1/xsl/params.xsl`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/chart example.html` & `jaraco.site-6.8.0/jaraco/site/templates/chart example.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/master.html` & `jaraco.site-6.8.0/jaraco/site/templates/master.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/openid/about.html` & `jaraco.site-6.8.0/jaraco/site/templates/openid/about.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/openid/id.html` & `jaraco.site-6.8.0/jaraco/site/templates/openid/id.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/openid/yadis.html` & `jaraco.site-6.8.0/jaraco/site/templates/openid/yadis.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/templates/welcome.html` & `jaraco.site-6.8.0/jaraco/site/templates/welcome.html`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco/site/ubuntu/nginx config` & `jaraco.site-6.8.0/jaraco/site/ubuntu/nginx config`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/jaraco.site.egg-info/PKG-INFO` & `jaraco.site-6.8.0/jaraco.site.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.site
-Version: 6.7.0
+Version: 6.8.0
 Summary: jaraco.com main website
 Home-page: https://github.com/jaraco/jaraco.site
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.site-6.7.0/jaraco.site.egg-info/SOURCES.txt` & `jaraco.site-6.8.0/jaraco.site.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/pytest.ini` & `jaraco.site-6.8.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/setup.cfg` & `jaraco.site-6.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.site-6.7.0/tox.ini` & `jaraco.site-6.8.0/tox.ini`

 * *Files identical despite different names*

