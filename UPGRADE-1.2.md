# UPGRADE FROM 1.1 to 1.2

* __BC BREAK:__ `Sylius\Bundle\UserBundle\Controller\UserController`'s method `addFlash` has been renamed to
  `addTranslatedFlash` with added scalar typehints for compatibility with both Symfony 3.4 and Symfony 4.0.

* The deprecated form mapping feature in SonataCoreBundle has been disabled in the app configuration included from SyliusCoreBundle.
  If you depend on the feature in your application, you will need to make the necessary changes. Refer to
  https://github.com/sonata-project/SonataCoreBundle/pull/462 for more information. 