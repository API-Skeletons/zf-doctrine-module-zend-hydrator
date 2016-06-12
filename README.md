Doctrine Zend Hydrator
======================

Since the zendframework/zend-stdlib hydrators into their own repository zendframework/zend-hydrator the DoctrineModule has not been updated to correctly use the new library.  Through many discussions on the issue Doctrine continues to maintain they are in line with zend-hydrator because, very unusually, the new library was written to be backwards compatible with zend-stdlib but that backwards compatibility was removed from zend-hydrator in later versions leaving developers who want to use Doctrine in their projects which allow for custom hydrators out on a limb.

This library overrides the files from DoctrineModule which are broken because of its implementation.  

Discussion on this issue:
 * Jan 30, 2016: https://github.com/doctrine/DoctrineModule/pull/548
 * Apr 7, 2016: https://github.com/doctrine/DoctrineModule/pull/558#issuecomment-207212246
