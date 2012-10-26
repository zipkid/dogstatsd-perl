dogstatsd-perl
==============

A Perl client for DogStatsd

Usage
----

    use DataDog::DogStatsd;

    $stat = DataDog::DogStatsd->new;

    $stat->increment( 'user.login', { tags => [ $s->cs->param( 'loginName' ) ] } );
