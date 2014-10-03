use Rex -feature => ['0.53'];

# Load Apache Module
use Apache;

desc "Setup Apache";
task "setup",
  group => "webserver",
  make {
  my $vhosts = get cmdb "virtual_hosts";
  Apache::setup;
  Apache::vhost $vhosts;
  };

1;
