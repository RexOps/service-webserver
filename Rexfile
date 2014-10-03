use Rex -feature => ['0.54'];

# Load Apache Module
use Apache;

desc "Setup Apache";
task "setup", make {
  my $vhosts = get cmdb "virtual_hosts";
  Apache::setup;
  Apache::vhost $vhosts;
};

1;
