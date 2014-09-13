use Rex -feature => ['0.51'];

# Load Apache Module
use Apache;

desc "Setup Apache";
task "setup",
  group => "webserver",
  make {
  my $vhosts = get cmdb "virtual_hosts";
  setup Apache;
  Apache::vhost $vhosts;
  };

1;
