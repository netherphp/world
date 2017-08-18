# Nether World (Current Version: v3.y.z)

A meta package to include all the things. This package will require verisons that do not
break backwards compat from the previous release of this package. This makes sense in my
head but let me elaborate just in case.

# About Versioning

Do not just copy this line. Note the current version series above.

	require { "netherphp/world": "^x.y.z" }

This will include the entire Nether stack and allow the individual components of the
stack to update as is. This does not nessessarily mean that all of the Nether packages
are in the 1.0.x zone. For example, as of this writing Surface and OneScript are already
in the 1.1.x zone.

The next time THIS package updates it will be 1.1.0 or 2.0.0 - so composer update will
still be safe for you because the way "^1.0.0" works, it will not allow 1.1.0 or 2.0.0.
Patch releases (0.0.x) will happen automatically for you on composer update. Minor
releases (0.x.x) will not happen automatically against "^1.0.0" so when Nether World goes
to 1.1.8 or whatever, you will need to update your composer to "^1.1.0" if you are
ready to deal with the BC changes.

I don't know if that made sense. But if you are using Nether World to just get all the
things use the ^#.#.0 syntax and you will always stay up to date with each component
without backwards compat breakages.
