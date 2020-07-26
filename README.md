# net-ntptime-perl
Perl 5 module to retrieve NTP and UNIX timestamp (unsigned integer) from an NTP server

Brandon Bourret (phatwares@cpan.org)

SYNOPSIS

use Net::NTPTime;

my $unix_time = get_unix_time;

my $unix_time = get_unix_time('ntp.server.com');

my $ntp_time = get_ntp_time;

my $ntp_time = get_ntp_time('ntp.server.com');

Pollutes the namespace with two functions: get_unix_time & get_ntp_time

METHODS

get_unix_time(OPTIONAL_NTP_SERVER)

Returns an integer timestamp indicating the number of elapsed seconds since 00:00 01-JAN-1970. You may include a specific NTP server to ping, or a default server will be used.

get_ntp_time(OPTIONAL_NTP_SERVER)

Returns an integer timestamp indicating the number of elapsed seconds since 00:00 01-JAN-1900. You may include a specific NTP server to ping, or a default server will be used.

Version History

1.00 - Initial Release

1.01 - Bug fix (changed "require Socket" to "use Socket")

1.02 - Fixed this POD document
Author

1.03 - More documentation fixes

Permission is granted to use this software under the same terms as Perl itself.

Refer to the Perl Artistic license for details.

Credits

The real credit goes to Tim Hogard for writing the code to do this. Thanks!
