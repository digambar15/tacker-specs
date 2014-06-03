===============================
OpenStack Tacker Specifications
===============================

NOTE:As Tacker is at early stage, it would be too early to apply the following
stuff. the following will be applied at some point when Tacker project matures
enough. The followings are copied from neutron-specs.


This git repository is used to hold approved design specifications for additions
to the Tacker project.  Reviews of the specs are done in gerrit, using a
similar workflow to how we review and merge changes to the code itself.

The layout of this repository is::

  specs/<release>/

You can find an example spec in `doc/source/specs/template.rst`. A
skeleton that contains all the sections required for a spec
file is located in `doc/source/specs/skeleton.rst` and can
be copied, then filled in with the details of a new blueprint for
convenience.

Specifications are proposed for a given release by adding them to the
`specs/<release>` directory and posting it for review.  The implementation
status of a blueprint for a given release can be found by looking at the
blueprint in launchpad.  Not all approved blueprints will get fully implemented.

Specifications have to be re-proposed for every release.  The review may be
quick, but even if something was previously approved, it should be re-reviewed
to make sure it still makes sense as written.

Please note, Launchpad blueprints are still used for tracking the
current status of blueprints. For more information, see::

  https://wiki.openstack.org/wiki/Blueprints

For more information about working with gerrit, see::

  https://wiki.openstack.org/wiki/Gerrit_Workflow

To validate that the specification is syntactically correct (i.e. get more
confidence in the Jenkins result), please execute the following command::

  $ tox

After running ``tox``, the documentation will be available for viewing in HTML
format in the ``doc/build/`` directory. Please do not checkin the generated
HTML files as a part of your commit.
