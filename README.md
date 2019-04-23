# Add Log Off Function

* This project provides a function implements a "log off" function for end users.
* A log off icon is added to the toolbar at the top of the screen, which logs out the user and reloads the login screen.
* Until now, when switching between DB information and login user information, it was necessary to log out from Aras Innovator, but by using this log off function, it's possible to log out and start up the browser. The trouble of displaying the Aras Innovator login page is eliminated, and efficiency is improved in development and testing.

* Aras Innovatorの開発者・ユーザー側の視点に立っての機能として、「ログオフ」機能を実装してい ます。
* 画面上部のツールバーに「ログオフ」のアイコンを新規に追加し、クリックすることでログイン画面に 戻る ことができます。
* 今までは、DB情報や、ログインユーザ情報を切り替える際に、一度Aras Innovatorから 「ログアウ ト」する必要がありましたが、 この「ログオフ」機能を用いれば、「ログアウト」→「ブラウザ立ち 上げ」→「 Aras Innovatorログインページの表示」の手間が無くなり、 開発やテストを行う上で効率が上がります。

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v1.0.0](https://github.com/ArasLabs/add-log-off-function/releases/tag/v1.0.0) | Support version 11SP6. Instructions are described in the ReadMe.pdf.

#### Supported Aras Versions

Project | Aras
--------|------
[v1.0.0](https://github.com/ArasLabs/add-log-off-function/releases/tag/v1.0.0) | 11.0 SP6

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **AddLogOffFunction** import package

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\AddLogOffFunction\Import\imports.mf` file in the Manifest File field.
6. Select **ExtCommon**, **jp.co.neo.Logoff**, **com.aras.innovator.cui_default** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

## Usage

Review the [ReadMe-LogoffAddFunc.pdf](./Documentation/ReadMe-LogoffAddFunc.pdf) for information on using the project. {[English translation](./Documentation/ReadMe-LogoffAddFunc-English.docx)}

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Created by NEOSYSTEM Co., Ltd.
