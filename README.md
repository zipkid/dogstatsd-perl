[![Build Status](https://travis-ci.org/binary-com/dogstatsd-perl.svg?branch=master)](https://travis-ci.org/binary-com/dogstatsd-perl)
[![Coverage Status](https://coveralls.io/repos/binary-com/dogstatsd-perl/badge.png?branch=master)](https://coveralls.io/r/binary-com/dogstatsd-perl?branch=master)

# NAME

DataDog::DogStatsd - A Perl client for DogStatsd

# SYNOPSIS

        use DataDog::DogStatsd;

        my $stat = DataDog::DogStatsd->new;
        $stat->increment( 'user.login', { tags => [ $s->cs->param( 'loginName' ) ] } );

# DESCRIPTION

DataDog::DogStatsd is a Perl client for DogStatsd

# METHODS

## new

- host

    default to 127.0.0.1

- port

    default to 8125

- namespace

    default to ''

## increment

        $stat->increment( 'user.login' );
        $stat->increment( 'user.login', { tags => [ $s->cs->param( 'loginName' ) ] } );
