dogstatsd-perl
==============

A Perl client for DogStatsd

Usage
----

    use DataDog::DogStatsd;

    $stat = DataDog::DogStatsd->new;

    $stat->_Stat->increment( 'user.login', { tags => [ $s->cs->param( 'loginName' ) ] } );
