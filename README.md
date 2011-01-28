# gitosis-webhook

GitHub style post-receive webhooks for gitosis.


## Requirements

To run this script on your server, you will need to have your own installation of [gitosis][1].


## Installation

This script is designed to be run on a private installation of gitosis as a post-receive hook for your repositories. To install this on your own server, simply drop the `post-receive` file into the `hooks` directory of your repository. You will need to give your gitosis user full read, write, and execute permissions on this file, which you can do by running `chmod 777 post-receive` from your terminal.


## Usage

The first line of this script allows you to specify a URL to which a JSON payload containing information about your commits is will be delivered via HTTP POST after each successful push to your repository. The format of this JSON payload matches the format used by [GitHub's post-receive webhooks][2].


## Disclaimer

Use this script at your own risk. While this script has been tested thoroughly, on the above requirements, your mileage may vary. I take no responsibility for any harmful actions this script might cause.


## License

This software, and its dependencies, are distributed free of charge and licensed under the GNU General Public License v3. For more information about this license and the terms of use of this software, please review the LICENSE.txt file.

[1]: http://eagain.net/gitweb/?p=gitosis.git
[2]: http://help.github.com/post-receive-hooks/
