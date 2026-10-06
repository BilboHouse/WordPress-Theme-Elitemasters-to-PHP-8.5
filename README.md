# Elite Masters for PHP 8.3–8.5

A community-maintained copy of the **Elite Masters** WordPress theme (upstream version 1.2) with automated PHP 8.3, 8.4, and 8.5 compatibility checks and an installable build.

The theme's original metadata identifies GT3Themes as its author and declares GPL-3.0. This repository is independent and is not an official GT3Themes project. Existing theme notices and third-party notices are retained.

## Install

1. Open the repository's [latest successful PHP compatibility workflow](https://github.com/BilboHouse/WordPress-Theme-Elitemasters-to-PHP-8.5/actions/workflows/php.yml).
2. Select the latest successful run on `main`.
3. Download the `elitemasters-php-8.3-8.5` artifact and extract it once.
4. In WordPress, go to **Appearance → Themes → Add New → Upload Theme**, select the extracted ZIP, and activate it.

The workflow artifact contains the theme files in a directly installable ZIP. No password is set. You can also clone or download this repository, but the GitHub source archive includes repository files such as this README and is not the installable package.

## PHP compatibility checks

GitHub Actions runs on every pull request to `main` and on pushes to `main`. It:

- Runs PHP syntax lint over the theme's PHP files with PHP 8.3, 8.4, and 8.5.
- Scans non-empty PHP files with PHPCompatibility targeting PHP 8.3–8.5.
- Builds the installable theme ZIP only after those checks pass.

The automated checks cover PHP code in this repository. They do not inspect PHP contained inside bundled plugin archives, test the theme with every WordPress/plugin combination, or replace visual and functional testing on a staging site. PHP version compatibility does not itself guarantee compatibility with a specific plugin or hosting configuration.

## Scope

The compatibility update preserves the theme's templates, styles, scripts, and behavior. No WordPress core or plugin files are modified by this project. Changes to the theme itself should be limited to PHP compatibility fixes and should retain the existing design and behavior.

Please report reproducible PHP compatibility issues with the PHP version, WordPress version, steps to reproduce, and relevant error log excerpt. Remove private paths, credentials, personal data, and production URLs before posting logs publicly.

## Attribution and licensing

Elite Masters theme metadata credits **mad_dog / GT3Themes** and declares **GPL-3.0**. Refer to the original theme files and bundled third-party components for their respective copyright and license notices. This repository does not claim ownership of the original theme.
