# ansible-test

The main tool for testing collections is ansible-test, Ansible’s testing tool described in [Testing Ansible](https://docs.ansible.com/ansible/latest/dev_guide/testing.html#developing-testing) and provided by both the ansible and ansible-core packages.

## Types of Tests:

- Sanity test:

According to Wikipedia, a sanity test is a basic test used to quickly evaluate whether a claim or calculation result could possibly be true. In the context of Ansible, these tests are used to ensure that all rules for creating and contributing to Ansible are satisfied.
For example like some rules describe for [Module format and documentation](https://docs.ansible.com/ansible/latest/dev_guide/developing_modules_documenting.html#module-documenting). See the full list of [Sanity Tests](https://docs.ansible.com/ansible/latest/dev_guide/testing/sanity/index.html#all-sanity-tests), which details the various tests and details how to fix identified issues. For information on how to run these tests, see [sanity testing guide](https://docs.ansible.com/ansible/latest/dev_guide/testing_sanity.html#testing-sanity). You can view all Ansible sanity tests by:
```
ansible-test sanity --list-tests
```

- Unit test:

Unit tests are small isolated tests that target a specific library or module. Unit tests in Ansible are currently the only way of driving tests from python within Ansible’s continuous integration process. This means that in some circumstances the tests may be a bit wider than just units. Unit tests can be found in test/units.

If you are running ansible-test with the --docker or --venv option you do not need to install dependencies manually. Otherwise you can install dependencies using the --requirements option.
Tests can either be written a simple functions or as classes. You can specify Python requirements in the tests/unit/requirements.txt file.

- Integration test:

[Tests for playbooks, by playbooks](https://docs.ansible.com/ansible/latest/dev_guide/testing_integration.html#testing-integration). Some tests may require credentials. Credentials may be specified with credentials.yml. Since integration tests can install requirements, and set-up, start and stop services, ansible documentation recommended running them in docker containers or otherwise restricted environments whenever possible. You must place integration tests in the appropriate tests/integration/targets/ directory.

## ansible-test cli

[Testing collections](https://docs.ansible.com/ansible/latest/dev_guide/developing_collections_testing.html#testing-collections) is short and very good review ansible-test cli and three types of tests: sanity, unit and integration.

```
ansible-test sanity
ansible-test units --docker
ansible-test units --python 2.7 --requirements apache2_module
ansible-test units --coverage apt
ansible-test coverage html
ansible-test integration --docker fedora35 -v
```

## How to Prepare the Environment for Tests

Most ansible-test commands support running in one or more isolated test environments to simplify testing. Containers(docker and podman), remote virtual machines, python virtual environments and composite environment arguments are options for test environments. More details for setup test environment are found [here](https://docs.ansible.com/ansible/latest/dev_guide/testing_running_locally.html#additional-requirements).
The [list of supported docker images](https://github.com/ansible/ansible/blob/devel/test/lib/ansible_test/_data/completion/docker.txt) for all options.

## How to Write Unit and Integration Tests

[Unit Testing Ansible Modules](https://docs.ansible.com/ansible/latest/dev_guide/testing_units_modules.html#testing-units-modules) explain when and why we need writing tests. [Mock](https://docs.python.org/3/library/unittest.mock.html) objects can be very useful in building unit tests. [Pytest](docs.pytest.org) framework makes it easy to write small, readable tests, and can scale to support complex functional testing for applications and libraries.

## Ansible codecov

[The online code coverage reports](https://app.codecov.io/gh/ansible/ansible) are a good way to identify areas for testing improvement in Ansible. 

[Code coverage](https://docs.ansible.com/ansible/latest/dev_guide/testing_running_locally.html#code-coverage) reports make it easy to identify untested code for which more tests should be written. Online reports are available but only cover the devel branch. For new code local reports are needed.Reports can be generated in several different formats.