dogstatsd-perl
==============

A Perl client for DogStatsd

Maintenance of this module has been taken over by Binary.com

They have also published this on CPAN

The newest version can be found at :

https://github.com/binary-com/dogstatsd-perl


Usage
----

    use DataDog::DogStatsd;

    $stat = DataDog::DogStatsd->new;

    $stat->increment( 'user.login', { tags => [ $s->cs->param( 'loginName' ) ] } );
