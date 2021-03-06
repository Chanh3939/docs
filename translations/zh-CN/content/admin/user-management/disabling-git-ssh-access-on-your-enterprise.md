---
title: Disabling Git SSH access on your enterprise
redirect_from:
  - /enterprise/admin/hidden/disabling-ssh-access-for-a-user-account/
  - /enterprise/admin/articles/disabling-ssh-access-for-a-user-account/
  - /enterprise/admin/hidden/disabling-ssh-access-for-your-appliance/
  - /enterprise/admin/articles/disabling-ssh-access-for-your-appliance/
  - /enterprise/admin/hidden/disabling-ssh-access-for-an-organization/
  - /enterprise/admin/articles/disabling-ssh-access-for-an-organization/
  - /enterprise/admin/hidden/disabling-ssh-access-to-a-repository/
  - /enterprise/admin/articles/disabling-ssh-access-to-a-repository/
  - /enterprise/admin/guides/installation/disabling-git-ssh-access-on-github-enterprise/
  - /enterprise/admin/installation/disabling-git-ssh-access-on-github-enterprise-server
  - /enterprise/admin/user-management/disabling-git-ssh-access-on-github-enterprise-server
  - /admin/user-management/disabling-git-ssh-access-on-github-enterprise-server
intro: 'You can prevent people from using Git over SSH for certain or all repositories on your enterprise.'
versions:
  enterprise-server: '*'
  github-ae: '*'
---

### 禁止对特定仓库进行 Git SSH 访问

{% data reusables.enterprise_site_admin_settings.override-policy %}

{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.repository-search %}
{% data reusables.enterprise_site_admin_settings.click-repo %}
{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.admin-top-tab %}
{% data reusables.enterprise_site_admin_settings.admin-tab %}
1. 在“Git SSH access”下，使用下拉菜单，然后单击 **Disabled**。 ![选择了禁用选项的 Git SSH access 下拉菜单](/assets/images/enterprise/site-admin-settings/git-ssh-access-repository-setting.png)

### 禁止对用户或组织拥有的所有仓库进行 Git SSH 访问

{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.search-user-or-org %}
{% data reusables.enterprise_site_admin_settings.click-user-or-org %}
{% data reusables.enterprise_site_admin_settings.access-settings %}
{% data reusables.enterprise_site_admin_settings.admin-top-tab %}
{% data reusables.enterprise_site_admin_settings.admin-tab %}
7. 在“Git SSH access”下，使用下拉菜单，然后单击 **Disabled**。 然后选择 **Enforce on all repositories**。 ![选择了禁用选项的 Git SSH access 下拉菜单](/assets/images/enterprise/site-admin-settings/git-ssh-access-organization-setting.png)

### Disabling Git SSH access to all repositories in your enterprise

{% data reusables.enterprise-accounts.access-enterprise %}
{% if currentVersion ver_gt "enterprise-server@2.21" or currentVersion == "github-ae@latest" %}
{% data reusables.enterprise-accounts.policies-tab %}
{% else %}
{% data reusables.enterprise-accounts.settings-tab %}
{% endif %}
{% data reusables.enterprise-accounts.options-tab %}
7. 在“Git SSH access”下，使用下拉菜单，然后单击 **Disabled**。 然后选择 **Enforce on all repositories**。 ![选择了禁用选项的 Git SSH access 下拉菜单](/assets/images/enterprise/site-admin-settings/git-ssh-access-appliance-setting.png)
