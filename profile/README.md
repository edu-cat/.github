# EduCat
Education program

[![Course Build](https://github.com/edu-cat/php-trainee-template/actions/workflows/course_build.yml/badge.svg?branch=master)](https://github.com/edu-cat/php-trainee-template/actions/workflows/course_build.yml)

# Table of Contents
1. [Greetings](#greetings)
2. [Pre-requirements](#pre-requirements)
3. [Workflow](#workflow)
4. [Special Notes](#special-notes)
5. [See also](#see-also)

## Greetings

Hello, my name is **Lyavon**. I'm **Professor Cat** and founder of the _EduCat Academy for Gifted Youngsters_.

This platform acts as an educational and training ground for cultivating Youngsters IT-powers.

I was created with love by [Dzianis Kotau - PHP Evangelist](https://dzianiskotau.com/) 
and [Yana Barantsava - Coolest Designer](https://uhovangoga.ru/). 

## Pre-requirements

1. It's highly recommended to use Ubuntu latest stable edition.
2. Install `php 8.1` following instructions for your OS.
3. Install and enable  at least `php-xml` extension.
4. Install [Composer tool](https://getcomposer.org/download/).
    - If you are using GNU/Linux, run as the last Composer installation step:
   ```bash
   mv composer.phar /usr/local/bin/composer
   chmod a+x /usr/local/bin/composer
   ```
5. Optional steps if you don't yet have public/private keys for your GitHub account:
    - Generate public/private keys for Github. You can use `ssh-keygen` command with parameters on GNU/Linux
      (press `Enter` for any prompt):
   ```bash
   ssh-keygen -t ecdsa -b 521 -C "educat_key" -f ~/.ssh/github_educat
   ```
    - Create `~/.ssh/config` file with following instructions:
   ```
   # GitHub.com
   Host github.com
   UpdateHostKeys no
   PreferredAuthentications publickey
   IdentityFile ~/.ssh/github_educat
   ```
    - [Copy](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
      ssh public key to your GitHub profile.
6. Identify yourself for GitHub:
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email"
```

## Workflow
1. You will be granted access to the repository with tasks.
2. Clone the repository to your machine.
3. Subscribe to the repository to be able to receive any notification on it.
4. Create separate branch and folder in src/ and tests/ for each task.
5. When you are ready to show your solution (task and tests), create Pull Request (PR).
6. If you have errors reported by GitHub Actions, check their details and fix issues.

## Special Notes
1. See Task1 [source](https://github.com/edu-cat/php-trainee-template/blob/master/src/Task1/myTernary.php) 
and [test](https://github.com/edu-cat/php-trainee-template/blob/master/tests/Task1/MyTernaryTest.php) 
files as example.
2. Use [PSR-12](https://www.php-fig.org/psr/psr-12/) and [PSR-4](https://www.php-fig.org/psr/psr-4/)
for code styling, autoload, etc.
3. Use English for comments, class, properties, methods, functions, etc.
4. If you use files without class declaration, add your src file to `lib/includes.php` file to be able to run tests.
5. Before creating PR run in your machine following commands

    - `composer style` to check code style
    - `composer analyse` to perform static analyse
    - `composer tests` to run tests
    - `composer validate --strict` to validate your composer config files

6. Create PR only after all above commands run with green (success) return status.

## See also
1. [PHP Documentation](https://www.php.net/docs.php)
2. [PHP: The Right Way](https://phptherightway.com/)
3. [Laracasts](https://laracasts.com/)
4. [SymfonyCasts](https://symfonycasts.com/)
5. [Laravel Daily](https://laraveldaily.com/)
6. [PHP Point](https://www.youtube.com/c/PHPPoint/videos)
7. [Composer](https://getcomposer.org/)
8. [Git Book](https://git-scm.com/book/en/v2)
