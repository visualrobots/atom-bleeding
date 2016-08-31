# Maintainer: Nicola Squartini <tensor5@gmail.com>
#             Brenton Horne <brentonhorne77 at gmail dot com>
_atom_url="https://github.com/atom"
_fus_url="https://github.com/fusion809"
_lee_url="https://github.com/lee-dohm"
_mur_url="https://github.com/Murriouz"
_language_patch2_url="${_fus_url}/language-patch2"
_ELECTRON_VERSION=$(</usr/lib/electron/version)
export _ELECTRON_VERSION=${_ELECTRON_VERSION#v}
export _NODE_VERSION=$(node --version | sed 's/v//g')

pkgname=atom-bleeding
_pkgname=atom
_apmver=1.12.6
_atomver=1.9.9
pkgver=${_atomver}.apm${_apmver}.e${_ELECTRON_VERSION}.n${_NODE_VERSION}
pkgrel=1
pkgdesc='A hackable text editor for the 21st Century built using web technologies on the Electron framework. Built with the latest versions of all bundled packages.'
arch=('i686' 'x86_64')
url="${_atom_url}/atom"
license=('MIT' 'custom')
conflicts=('apm-bleeding')
provides=('apm-bleeding')
depends=('electron'
         'python-pylint'
         'python2-pylint'
         'clang'
         'namcap'
         'npm'
         'lua'
         'libgnome-keyring'
         'nodejs'
         'python2'
         'coffee-script'
         'java-environment')
optdepends=('ctags: symbol indexing support')
makedepends=('coffee-script' 'git')
# git sources
source=("about-arch::git+${_fus_url}/about.git"
        "atom::git+${url}.git"
        "ask-stack::git+https://github.com/Chris911/Ask-Stack-Atom.git"
        "dark-bint-syntax::git+${_mur_url}/dark-bint-syntax.git"
        "fusion-ui::git+${_fus_url}/fusion-ui.git"
        "file-icons::git+https://github.com/DanBrooker/file-icons.git"
        "language-archlinux::git+${_fus_url}/language-archlinux.git"
        "language-gfm2::git+${_fus_url}/language-gfm2.git"
        "language-ini-desktop::git+${_fus_url}/language-ini-desktop.git"
        "language-liquid::git+https://github.com/puranjayjain/language-liquid.git"
        "language-patch2::git+${_fus_url}/language-patch2.git"
        "language-unix-shell::git+${_fus_url}/language-shellscript.git"
        "language-vala-modern::git+${_fus_url}/language-vala-modern.git"
        "terminal-fusion::git+${_fus_url}/terminal-fusion.git"
        "apm::git+https://github.com/atom/apm.git"
        "archive-view::git+${_atom_url}/archive-view.git"
        "autocomplete-atom-api::git+${_atom_url}/autocomplete-atom-api.git"
        "autocomplete-clang::git+https://github.com/yasuyuky/autocomplete-clang.git"
        "autocomplete-css::git+${_atom_url}/autocomplete-css.git"
        "autocomplete-java::git+https://github.com/keskiju/autocomplete-java.git"
        "autocomplete-html::git+${_atom_url}/autocomplete-html.git"
        "autocomplete-modules::git+https://github.com/nkt/atom-autocomplete-modules.git"
        "autocomplete-plus::git+${_atom_url}/autocomplete-plus.git"
        "autocomplete-python::git+https://github.com/sadovnychyi/autocomplete-python.git"
        "autocomplete-sass::git+https://github.com/saschagehlich/autocomplete-sass.git"
        "autocomplete-snippets::git+${_atom_url}/autocomplete-snippets.git"
        "autoflow::git+${_atom_url}/autoflow.git"
        "autosave::git+${_atom_url}/autosave.git"
        "background-tips::git+${_atom_url}/background-tips.git"
        "bookmarks::git+${_atom_url}/bookmarks.git"
        "bracket-matcher::git+${_atom_url}/bracket-matcher.git"
        "command-palette::git+${_atom_url}/command-palette.git"
        "deprecation-cop::git+${_atom_url}/deprecation-cop.git"
        "dev-live-reload::git+${_atom_url}/dev-live-reload.git"
        "encoding-selector::git+${_atom_url}/encoding-selector.git"
        "fuzzy-finder::git+${_atom_url}/fuzzy-finder.git"
        "git-diff::git+${_atom_url}/git-diff.git"
        "git-plus::git+https://github.com/akonwi/git-plus.git"
        "git-time-machine::git+https://github.com/littlebee/git-time-machine.git"
        "gpp-compiler::git+https://github.com/kriscross07/atom-gpp-compiler.git"
        "find-and-replace::git+${_atom_url}/find-and-replace.git"
        "go-to-line::git+${_atom_url}/go-to-line.git"
        "grammar-selector::git+${_atom_url}/grammar-selector.git"
        "hyperclick::git+https://github.com/facebooknuclideapm/hyperclick.git"
        "hyperlink-hyperclick::git+https://github.com/UziTech/hyperlink-hyperclick.git"
        "image-view::git+${_atom_url}/image-view.git"
        "incompatible-packages::git+${_atom_url}/incompatible-packages.git"
        "keybinding-resolver::git+${_atom_url}/keybinding-resolver.git"
        "line-ending-selector::git+${_atom_url}/line-ending-selector.git"
        "markdown-preview::git+${_atom_url}/markdown-preview.git"
        "minimap::git+https://github.com/atom-minimap/minimap.git"
        "notifications::git+${_atom_url}/notifications.git"
        "open-on-github::git+${_atom_url}/open-on-github.git"
        "package-generator::git+${_atom_url}/package-generator.git"
        "pigments::git+https://github.com/abe33/atom-pigments.git"
        "script::git+https://github.com/rgbkrk/atom-script.git"
        "settings-view::git+${_atom_url}/settings-view.git"
        "snippets::git+${_atom_url}/snippets.git"
        "spell-check::git+${_atom_url}/spell-check.git"
        "status-bar::git+${_atom_url}/status-bar.git"
        "styleguide::git+${_atom_url}/styleguide.git"
        "symbols-view::git+${_atom_url}/symbols-view.git"
        "tabs::git+${_atom_url}/tabs.git"
        "timecop::git+${_atom_url}/timecop.git"
        "tool-bar::git+https://github.com/suda/tool-bar.git"
        "toolbar-fusion::git+${_fus_url}/toolbar-fusion.git"
        "tree-view::git+${_atom_url}/tree-view.git"
        "update-package-dependencies::git+${_atom_url}/update-package-dependencies.git"
        "welcome::git+${_atom_url}/welcome.git"
        "whitespace::git+${_atom_url}/whitespace.git"
        "wrap-guide::git+${_atom_url}/wrap-guide.git"
        "language-c::git+${_atom_url}/language-c.git"
        "language-clojure::git+${_atom_url}/language-clojure.git"
        "language-coffee-script::git+${_atom_url}/language-coffee-script.git"
        "language-csharp::git+${_atom_url}/language-csharp.git"
        "language-css::git+${_atom_url}/language-css.git"
        "language-docker::git+https://github.com/jagregory/language-docker.git"
        "language-git::git+${_atom_url}/language-git.git"
        "language-go::git+${_atom_url}/language-go.git"
        "language-html::git+${_atom_url}/language-html.git"
        "language-hyperlink::git+${_atom_url}/language-hyperlink.git"
        "language-java::git+${_atom_url}/language-java.git"
        "language-javascript::git+${_atom_url}/language-javascript.git"
        "language-json::git+${_atom_url}/language-json.git"
        "language-less::git+${_atom_url}/language-less.git"
        "language-lisp::git+https://github.com/enriquefernandez/language-lisp.git"
        "language-lua::git+https://github.com/FireZenk/language-lua.git"
        "language-make::git+${_atom_url}/language-make.git"
        "language-matlab-octave::git+https://github.com/thedavidprice/language-matlab-octave.git"
        "language-mustache::git+${_atom_url}/language-mustache.git"
        "language-objective-c::git+${_atom_url}/language-objective-c.git"
        "language-pascal::git+https://github.com/alefragnani/atom-language-pascal.git"
        "language-perl::git+${_atom_url}/language-perl.git"
        "language-php::git+${_atom_url}/language-php.git"
        "language-property-list::git+${_atom_url}/language-property-list.git"
        "language-python::git+${_atom_url}/language-python.git"
        "language-ruby::git+${_atom_url}/language-ruby.git"
        "language-ruby-on-rails::git+${_atom_url}/language-ruby-on-rails.git"
        "language-rust::git+https://github.com/zargony/atom-language-rust.git"
        "language-sass::git+${_atom_url}/language-sass.git"
        "language-scala::git+https://github.com/atom-community/language-scala.git"
        "language-source::git+${_atom_url}/language-source.git"
        "language-sql::git+${_atom_url}/language-sql.git"
        "language-text::git+${_atom_url}/language-text.git"
        "language-todo::git+${_atom_url}/language-todo.git"
        "language-toml::git+${_atom_url}/language-toml.git"
        "language-xml::git+${_atom_url}/language-xml.git"
        "language-yaml::git+${_atom_url}/language-yaml.git"
        "linter-clang::git+https://github.com/AtomLinter/linter-clang.git"
        "linter-coffeescript::git+https://github.com/hokaccha/linter-coffeescript.git"
        "linter-jsonlint::git+https://github.com/AtomLinter/linter-jsonlint.git"
        "linter-pylint::git+https://github.com/AtomLinter/linter-pylint.git"
        "linter-lua::git+https://github.com/AtomLinter/linter-lua.git")
# patches, json, js and desktop files
source+=('about-view.js'
'atom-bleeding.desktop'
'atom.sh'
'beforeunload.patch'
'deprecated-api.patch'
'fix-license-path.patch'
'fix-marker-index.patch'
'fix-oniguruma.patch'
'run-as-node.patch'
'theme.patch'
'tree-view.patch'
'use-system-apm.patch'
'use-system-electron.patch'
'apm.js'
'no-scripts.patch'
'upgrade.patch'
'fix-pane-resize-handle.patch'
'use-system-node-gyp.patch'
'symbols-view-use-system-ctags.patch')
sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            '4c18bd6bc068cd2aade7270941e2b75ac2264f73c5d28ba4f812cd7d48b37679'
            'f1b9e3e844dad4768b9f352198882dbc073e879d3eec1848a7001b5888715803'
            '17e19ac310007e6b9b4bcd78c13b2a8322909cac15375aacd14c079253930341'
            'e92e23bbf839bec6611b2ac76c1f5bba35b476983b0faa9b310288e2956247a2'
            '4b978622b98d18affcd02e389b8410f4a6d33865c4aa02567a72a5c2c3b7030d'
            '11237bea5c7551984226d6db1c2dc5650b47df66bc8eec5238e80a9259cbf669'
            'a8b1766ced19c1583915ff8b0ce8b7d96baef22e103fcdbffe9f9c8126ad4df4'
            '70ba93703dbdecbea106a92127e40d3c153e1fd9519cf1bfd12202bf49840c5e'
            'fb96c10f76a6e088c2c50c6ee0a68e01ca5f60943fe3879574c0aaae624d33a9'
            '9e990a69b2ce007eac3054fdb5ae9e42f60811a767d8aa37a10da614a5dd68a3'
            '109af01ceae45615994f2ac08292c44db339bf7ef89369b077e04fcfc35aa3dd'
            '7f81e7245c7099b69380aef9f9b79fcaca8384a5fa00e6767bbfe00b1f81935f'
            '0b380a4fb7399fb23dad23b7aacb3d4d603b436bac318bbbbc1641e2ff840f3b'
            '0e607fef2a1a92d58fa5b7beca2a059bdbcc7ecd4198013baa1ffd05fff5446e'
            '0763015eb5ddb8346a5cef3479d80023d32382531d8a651c230c8f2144ba3628'
            '4d73feaadc49d2daae4e3fffcd35d4d57608d03b622bc6fb0d9d16e71e43a6a2'
            '1d5a4e6f2f928ebea64ee70c8a6ecf1935a1409ca7e50b02c70ae9f3315328b6'
            'ce8d45831e3d5071b7b913e8d1a014ec3b1ac3586194039006dcf87c100cc189'
            'd6ce1a5e16a42aa50c89848f36eaf2e5ef07a93f36dc740eaeb6ac7a6b3e0432')

_pkgver() {
  function describe {
    printf "$(git -C "$srcdir/$1" describe --tags `git -C "$srcdir/$1" rev-list --tags --max-count=1` | sed 's/v//g')"
  }
  _about_arch_ver=$(describe about-arch)
  _apmver=$(describe apm)
  _archive_view_ver="$(describe archive-view)"
  _autocomplete_css_ver="$(describe autocomplete-css)"
  _autocomplete_modules_ver="$(describe autocomplete-modules)"
  _autocomplete_plus_ver="$(describe autocomplete-plus)"
  _autocomplete_sass_ver="$(describe autocomplete-sass)"
  _autocomplete_snippets_ver="$(describe autocomplete-snippets)"
  _background_tips_ver="$(describe background-tips)"
  _bookmarks_ver="$(describe bookmarks)"
  _bracket_matcher_ver="$(describe bracket-matcher)"
  _dark_bint_syntax_ver="$(describe dark-bint-syntax)"
  _encoding_selector_ver="$(describe encoding-selector)"
  _file_icons_ver="$(describe file-icons)"
  _find_and_replace_ver="$(describe find-and-replace)"
  _fusion_ui_ver="$(describe fusion-ui)"
  _fuzzy_finder_ver="$(describe fuzzy-finder)"
  _git_diff_ver="$(describe git-diff)"
  _git_plus_ver="$(describe git-plus)"
  _git_time_machine_ver="$(describe git-time-machine)"
  _go_to_line_ver="$(describe go-to-line)"
  _gpp_compiler_ver="$(describe gpp-compiler)"
  _grammar_selector_ver="$(describe grammar-selector)"
  _hyperclick_ver="$(describe hyperclick)"
  _hyperlink_hyperclick_ver="$(describe hyperlink-hyperclick)"
  _image_view_ver="$(describe image-view)"
  _language_archlinux_ver="$(describe language-archlinux)"
  _language_c_ver="$(describe language-c)"
  _language_clojure_ver="$(describe language-clojure)"
  _language_coffee_script_ver="$(describe language-coffee-script)"
  _language_css_ver="$(describe language-css)"
  _language_docker_ver="$(describe language-docker)"
  _language_gfm2_ver="$(describe language-gfm2)"
  _language_git_ver="$(describe language-git)"
  _language_go_ver="$(describe language-go)"
  _language_html_ver="$(describe language-html)"
  _language_ini_desktop_ver="$(describe language-ini-desktop)"
  _language_java_ver="$(describe language-java)"
  _language_javascript_ver="$(describe language-javascript)"
  _language_json_ver="$(describe language-json)"
  _language_less="$(describe language-less)"
  _language_liquid_ver="$(describe language-liquid)"
  _language_make_ver="$(describe language-make)"
  _language_patch2_ver="$(describe language-patch2)"
  _language_perl_ver="$(describe language-perl)"
  _language_php_ver="$(describe language-php)"
  _language_python_ver="$(describe language-python)"
  _language_ruby_ver="$(describe language-ruby)"
  _language_rust_ver="$(describe language-rust)"
  _language_sass_ver="$(describe language-sass)"
  _language_sql_ver="$(describe language-sql)"
  _language_todo_ver="$(describe language-todo)"
  _language_unix_shell_ver="$(describe language-unix-shell)"
  _language_vala_modern_ver="$(describe language-vala-modern)"
  _language_xml_ver="$(describe language-xml)"
  _language_yaml_ver="$(describe language-yaml)"
  _line_ending_selector_ver="$(describe line-ending-selector)"
  _linter_ver="$(describe linter)"
  _linter_clang_ver="$(describe linter-clang)"
  _linter_coffeescript_ver="$(describe linter-coffeescript)"
  _linter_jsonlint_ver="$(describe linter-jsonlint)"
  _linter_lua_ver="$(describe linter-lua)"
  _markdown_preview_ver="$(describe markdown-preview)"
  _minimap_ver="$(describe minimap)"
  _notifications_ver="$(describe notifications)"
  _open_on_github_ver="$(describe open-on-github)"
  _pigments_ver="$(describe pigments)"
  _script_ver="$(describe script)"
  _settings_view_ver="$(describe settings-view)"
  _snippets_ver="$(describe snippets)"
  _spell_check_ver="$(describe spell-check)"
  _styleguide_ver="$(describe styleguide)"
  _symbols_view_ver="$(describe symbols-view)"
  _tabs_ver="$(describe tabs)"
  _timecop_ver="$(describe timecop)"
  _tf_ver="$(describe terminal-fusion)"
  _tree_view_ver="$(describe tree-view)"
  _whitespace_ver="$(describe whitespace)"

  printf "${_atomver}.aa${_about_arch_ver}.ac${_autocomplete_css_ver}.am${_autocomplete_modules_ver}.ap${_autocomplete_plus_ver}.apm${_apmver}.as${_autocomplete_sass_ver}.asn${_autocomplete_snippets_ver}.av${_archive_view_ver}.b${_bookmarks_ver}.bm${_bracket_matcher_ver}.bt${_background_tips_ver}.d${_dark_bint_syntax_ver}.e${_ELECTRON_VERSION}.es${_encoding_selector_ver}.ff${_fuzzy_finder_ver}.fi${_file_icons_ver}.fr${_find_and_replace_ver}.fu${_fusion_ui_ver}.g${_gpp_compiler_ver}.gd${_git_diff_ver}.gl${_go_to_line_ver}.gp${_git_plus_ver}.gs${_grammar_selector_ver}.gtm${_git_time_machine_ver}.iv${_image_view_ver}.l${_linter_ver}.la${_language_archlinux_ver}.lc${_linter_clang_ver}.lcs${_linter_coffeescript_ver}.ld${_language_docker_ver}.les${_line_ending_selector_ver}.lg${_language_gfm2_ver}.lgo${_language_go_ver}.lh${_language_html_ver}.li${_language_ini_desktop_ver}.lj${_linter_jsonlint_ver}.lja${_language_java_ver}.ljs${_language_javascript_ver}.ljso${_language_json_ver}.ll${_linter_lua_ver}.lld${_language_liquid_ver}.lle${_language_less_ver}.lm${_language_make_ver}.lp${_language_patch2_ver}.lph${_language_php_ver}.lpl${_language_perl_ver}.lpy${_language_python_ver}.lr${_language_ruby_ver}.lrt${_language_rust_ver}.ls${_la_language_sass_ver}.lsq${_language_sql_ver}.lt${_language_todo_ver}.lu${_language_unix_shell_ver}.lv${_language_vala_modern_ver}.lx${_language_xml_ver}.ly${_language_yaml_ver}.m${_minimap_ver}.mp${_markdown_preview_ver}.o${_open_on_github_ver}.p${_pigments_ver}.s${_script_ver}.sc${_spell_check_ver}.sev${_settings_view_ver}.sg${_styleguide_ver}.sv${_symbols_view_ver}.t${_tabs_ver}.tc${_timecop_ver}.tf${_tf_ver}.tv${_tree_view_ver}.w${_whitespace_ver}" | sed 's/-/./g'
}

prepare() {
  function describe {
    printf "$(git -C "$srcdir/$1" describe --tags `git -C "$srcdir/$1" rev-list --tags --max-count=1` | sed 's/v//g')"
  }
  _about_arch_ver=$(describe about-arch)
  _apmver=$(describe apm)
  _ask_stack_ver="$(describe ask-stack)"
  _autocomplete_clang_ver="$(describe autocomplete-clang)"
  _autocomplete_java_ver="$(describe autocomplete-java)"
  _autocomplete_python_ver="$(describe autocomplete-python)"
  _autocomplete_modules_ver="$(describe autocomplete-modules)"
  _autocomplete_sass_ver="$(describe autocomplete-sass)"
  _dark_bint_syntax_ver="$(describe dark-bint-syntax)"
  _file_icons_ver="$(describe file-icons)"
  _fusion_ui_ver="$(describe fusion-ui)"
  _git_plus_ver="$(describe git-plus)"
  _git_time_machine_ver="$(describe git-time-machine)"
  _gpp_compiler_ver="$(describe gpp-compiler)"
  _hyperclick_ver="$(describe hyperclick)"
  _hyperlink_hyperclick_ver="$(describe hyperlink-hyperclick)"
  _language_archlinux_ver="$(describe language-archlinux)"
  _language_docker_ver="$(describe language-docker)"
  _language_gfm2_ver="$(describe language-gfm2)"
  _language_ini_desktop_ver="$(describe language-ini-desktop)"
  _language_liquid_ver="$(describe language-liquid)"
  _language_lisp_ver="$(describe language-lisp)"
  _language_lua_ver="$(describe language-lua)"
  _language_matlab_octave_ver="$(describe language-matlab-octave)"
  _language_pascal_ver="$(describe language-pascal)"
  _language_patch2_ver="$(describe language-patch2)"
  _language_rust_ver="$(describe language-rust)"
  _language_scala_ver="$(describe language-scala)"
  _language_unix_shell_ver="$(describe language-unix-shell)"
  _language_vala_modern_ver="$(describe language-vala-modern)"
  _linter_clang_ver="$(describe linter-clang)"
  _linter_coffeescript_ver="$(describe linter-coffeescript)"
  _linter_jsonlint_ver="$(describe linter-jsonlint)"
  _linter_pylint_ver="$(describe linter-pylint)"
  _linter_lua_ver="$(describe linter-lua)"
  _minimap_ver="$(describe minimap)"
  _pigments_ver="$(describe pigments)"
  _script_ver="$(describe script)"
  _tool_bar_ver="$(describe tool-bar)"
  _toolbar_fusion_ver="$(describe toolbar-fusion)"
  _tf_ver="$(describe terminal-fusion)"

  ## apm
  rm -rf "${srcdir}"/apm-build
  sed -i -e "s/_this.installedAtomVersion = '.*'/_this.installedAtomVersion = '${_atomver}'/g" ${srcdir}/../upgrade.patch
  updpkgsums $srcdir/../PKGBUILD

  cd apm
  git checkout v${_apmver}
  # Use custom launcher
  rm bin/apm{,.cmd} bin/npm{,.cmd}
  rm src/cli.coffee
  install -m755 ${srcdir}/apm.js bin/apm

  # Don't download binary Node
  patch -Np1 -i ${srcdir}/no-scripts.patch
  rm BUNDLED_NODE_VERSION script/*

  # Use system node-gyp
  patch -Np1 -i ../use-system-node-gyp.patch

  ## atom
  cd "${srcdir}/${_pkgname}"
  git checkout v${_atomver}

  sed -e "s|<SRCDIR>|$srcdir/apm-build|g" "${srcdir}"/use-system-apm.patch > $srcdir/use-system-apm-fix.patch

  patch -Np1 -i "${srcdir}"/use-system-electron.patch
  patch -Np1 -i "${srcdir}"/use-system-apm-fix.patch
  patch -Np1 -i "${srcdir}"/fix-license-path.patch

  # apm with system (updated) nodejs cannot 'require' modules inside asar
  sed -e "s/, 'generate-asar'//" -i build/Gruntfile.coffee

  sed -i -e "/exception-reporting/d" \
         -e "/metrics/d" \
         -e "/-ui/d" \
         -e "/-syntax/d" \
         -e "/-theme/d" \
         -e "s/\"language-gfm\": \".*\",/\"language-gfm2\": \"${_language_gfm2_ver}\",\n    \"language-ini-desktop\": \"${_language_ini_desktop_ver}\",\n    \"language-liquid\": \"${_language_liquid_ver}\",\n    \"language-patch2\": \"${_language_patch2_ver}\",/g" \
         -e "/\"dependencies\": {/a \
                     \"language-patch2\": \"${_language_patch2_url}\"," \
         -e "s/\"language-shellscript\": \".*\",/\"language-lisp\": \"${_language_lisp_ver}\",\n    \"language-lua\": \"${_language_lua_ver}\",\n    \"language-matlab-octave\": \"${_language_matlab_octave_ver}\",\n    \"language-pascal\": \"${_language_pascal_ver}\",\n    \"language-rust\": \"${_language_rust_ver}\",\n    \"language-scala\": \"${_language_scala_ver}\",\n    \"language-unix-shell\": \"${_language_unix_shell_ver}\",\n    \"language-vala-modern\": \"${_language_vala_modern_ver}\",\n    \"language-archlinux\": \"${_language_archlinux_ver}\",\n    \"language-docker\": \"${_language_docker_ver}\",\n    \"terminal-fusion\": \"${_tf_ver}\",\n    \"tool-bar\": \"${_tool_bar_ver}\",\n    \"toolbar-fusion\": \"${_toolbar_fusion_ver}\",\n    \"linter-clang\": \"${_linter_clang_ver}\",\n    \"linter-coffeescript\": \"${_linter_coffeescript_ver}\",\n    \"linter-jsonlint\": \"${_linter_jsonlint_ver}\",\n    \"linter-pylint\": \"${_linter_pylint_ver}\",\n    \"linter-lua\": \"${_linter_lua_ver}\",/g" \
         -e "s/\"about\": \".*\"/\"about-arch\": \"${_about_arch_ver}\"/g" \
         -e "s/\"link\": \".*\",/\"hyperclick\": \"${_hyperclick_ver}\",\n    \"hyperlink-hyperclick\": \"${_hyperlink_hyperclick_ver}\",\n    \"minimap\": \"${_minimap_ver}\",\n    \"pigments\": \"${_pigments_ver}\",/g" \
         -e "/\"packageDependencies\": {/a \
              \"ask-stack\": \"${_ask_stack_ver}\",\n    \"autocomplete-clang\": \"${_autocomplete_clang_ver}\",\n    \"autocomplete-java\": \"${_autocomplete_java_ver}\",\n    \"autocomplete-modules\": \"${_autocomplete_modules_ver}\",\n    \"autocomplete-python\": \"${_autocomplete_python_ver}\",\n    \"autocomplete-sass\": \"${_autocomplete_sass_ver}\",\n    \"dark-bint-syntax\": \"${_dark_bint_syntax_ver}\",\n    \"file-icons\": \"${_file_icons_ver}\",\n    \"fusion-ui\": \"${_fusion_ui_ver}\",\n    \"gpp-compiler\": \"${_gpp_compiler_ver}\",\n    \"git-plus\": \"${_git_plus_ver}\",\n    \"git-time-machine\": \"${_git_time_machine_ver}\"," package.json

  _L=("archive-view"
  "autocomplete-atom-api"
  "autocomplete-css"
  "autocomplete-html"
  "autocomplete-plus"
  "autocomplete-snippets"
  "autoflow"
  "autosave"
  "background-tips"
  "bookmarks"
  "bracket-matcher"
  "command-palette"
  "deprecation-cop"
  "dev-live-reload"
  "encoding-selector"
  "fuzzy-finder"
  "git-diff"
  "find-and-replace"
  "go-to-line"
  "grammar-selector"
  "image-view"
  "incompatible-packages"
  "keybinding-resolver"
  "line-ending-selector"
  "markdown-preview"
  "notifications"
  "open-on-github"
  "package-generator"
  "settings-view"
  "snippets"
  "spell-check"
  "status-bar"
  "styleguide"
  "symbols-view"
  "tabs"
  "timecop"
  "tree-view"
  "update-package-dependencies"
  "welcome"
  "whitespace"
  "wrap-guide"
  "language-c"
  "language-clojure"
  "language-coffee-script"
  "language-csharp"
  "language-css"
  "language-git"
  "language-go"
  "language-html"
  "language-hyperlink"
  "language-java"
  "language-javascript"
  "language-json"
  "language-less"
  "language-make"
  "language-mustache"
  "language-objective-c"
  "language-perl"
  "language-php"
  "language-property-list"
  "language-python"
  "language-ruby"
  "language-ruby-on-rails"
  "language-sass"
  "language-source"
  "language-sql"
  "language-text"
  "language-todo"
  "language-toml"
  "language-xml"
  "language-yaml")

  for i in "${_L[@]}"
  do
    unset ver
    ver="$(git -C "$srcdir/$i" describe --tags `git -C "$srcdir/$i" rev-list --tags --max-count=1` | sed 's/v//g')"
    sed -i -e "s/\"$i\": \".*\"/\"$i\": \"$ver\"/g" package.json
  done

  # Fix for Electron 1.2.0
  patch -Np1 -i "${srcdir}"/beforeunload.patch
  patch -Np1 -i "${srcdir}"/run-as-node.patch

  # Fix for Electron 1.3.0
  patch -Np1 -i "${srcdir}"/fix-pane-resize-handle.patch

  # Theme patch
  patch -Np1 -i "${srcdir}"/theme.patch
}

build() {
  ## apm
  cd apm

  coffee -c --no-header -o lib src/*.coffee
  npm install --user root -g --prefix="${srcdir}"/apm-build/usr

  cd "${srcdir}/apm-build${_apmdir}"

  # Use system npm
  npm uninstall npm

  npm dedupe

  ## atom
  cd "${srcdir}/${_pkgname}"

  export ATOM_RESOURCE_PATH="$srcdir/${_pkgname}"
  # If unset, ~/.atom/.node-gyp/.atom/.npm is used
  export NPM_CONFIG_CACHE="${HOME}/.atom/.npm"

  # Make sure NodeGit builds from source and with the correct runtime
  export BUILD_ONLY=1
  export ELECTRON_VERSION=${_ELECTRON_VERSION}
  export APMBIN="$srcdir/apm-build/usr/lib/node_modules/atom-package-manager/bin/apm"

  LDFLAGS="${LDFLAGS} -Wl,-z,noexecstack" $APMBIN clean
  # -Wl,-z,noexecstack to make sure nodegit.node does not have executable stack
  LDFLAGS="${LDFLAGS} -Wl,-z,noexecstack" $APMBIN install

  # Fix for Node 6
  cd node_modules/autocomplete-clang/lib
  sed -i -e 's/.coffee//g' *.coffee
  cd ../../..
  # Use system ctags
  cd node_modules/symbols-view
  patch -Np1 -i "${srcdir}"/symbols-view-use-system-ctags.patch
  rm -r vendor
  cd ../..
  cd node_modules/tree-view
  patch -Np1 -i ${srcdir}/tree-view.patch
  cd ../..

  # Fix for Electron 1.3.0
  _node_gyp="node-gyp rebuild --target=${_ELECTRON_VERSION} --dist-url=https://atom.io/download/atom-shell"
  cd node_modules/marker-index
  patch -Np1 -i "${srcdir}"/fix-marker-index.patch
  ${_node_gyp}
  cd ../oniguruma
  patch -Np1 -i "${srcdir}"/fix-oniguruma.patch
  ${_node_gyp}
  cd ../../

  _packagesToDedupe=('abbrev'
                     'amdefine'
                     'atom-space-pen-views'
                     'cheerio'
                     'domelementtype'
                     'fs-plus'
                     'grim'
                     'highlights'
                     'humanize-plus'
                     'iconv-lite'
                     'inherits'
                     'loophole'
                     'oniguruma'
                     'q'
                     'request'
                     'rimraf'
                     'roaster'
                     'season'
                     'sigmund'
                     'semver'
                     'through'
                     'temp')

  LDFLAGS="${LDFLAGS} -Wl,-z,noexecstack" $APMBIN dedupe ${_packagesToDedupe[@]}
  cd build && npm install && cd ..
  LDFLAGS="${LDFLAGS} -Wl,-z,noexecstack" script/grunt --channel=stable
}

package() {
  ## apm
  cp -r "${srcdir}"/apm-build/usr "${pkgdir}"
  rm $pkgdir/usr/bin/apm
  cd $pkgdir/usr/bin/
  ln -sf ../lib/node_modules/atom-package-manager/bin/apm apm-bleeding

  cd "${pkgdir}"${_apmdir}

  install -dm755 ${pkgdir}/usr/share/doc/${pkgname}/apm/
  install -dm755 ${pkgdir}/usr/share/doc/${pkgname}/atom/
  install -Dm644 "${srcdir}"/apm/README.md ${pkgdir}/usr/share/doc/${pkgname}/apm/README.md
  install -Dm644 "${srcdir}"/atom/README.md ${pkgdir}/usr/share/doc/${pkgname}/atom/README.md
  install -Dm644 "${srcdir}/atom/package.json" "${pkgdir}/usr/share/doc/${pkgname}/atom/package.json"

  # Install license file
  install -d -m755 "${pkgdir}/usr/share/licenses/${pkgname}/{apm,atom}"
  ln -s ../../../lib/node_modules/atom-package-manager/LICENSE.md \
     "${pkgdir}/usr/share/licenses/${pkgname}/apm"

  # Remove occurrences of ${srcdir}
  find "${pkgdir}" -name "package.json" \
       -exec sed -e "s|${srcdir}/apm-build||" \
                 -e "s|${srcdir}/apm|${_apmdir}|" \
                 -i '{}' \;

  # Remove useless stuff
  find "${pkgdir}"/usr/lib \
      -name ".*" -prune -exec rm -r '{}' \; \
      -or -name "*.a" -exec rm '{}' \; \
      -or -name "*.bat" -exec rm '{}' \; \
      -or -name "*.mk" -exec rm '{}' \; \
      -or -path "*/git-utils/binding.gyp" -exec rm '{}' \; \
      -or -path "*/git-utils/src" -prune -exec rm -r '{}' \; \
      -or -path "*/keytar/binding.gyp" -exec rm '{}' \; \
      -or -path "*/keytar/src" -prune -exec rm -r '{}' \; \
      -or -path "*/oniguruma/binding.gyp" -exec rm '{}' \; \
      -or -path "*/oniguruma/src" -prune -exec rm -r '{}' \; \
      -or -name "*.yml" -exec rm '{}' \; \
      -or -name "benchmark" -prune -exec rm -r '{}' \; \
      -or -name "binding.Makefile" -exec rm '{}' \; \
      -or -name "config.gypi" -exec rm '{}' \; \
      -or -name "deps" -prune -exec rm -r '{}' \; \
      -or -name "doc" -prune -exec rm -r '{}' \; \
      -or -name "html" -prune -exec rm -r '{}' \; \
      -or -name "Makefile" -exec rm '{}' \; \
      -or -name "man" -prune -exec rm -r '{}' \; \
      -or -name "obj.target" -prune -exec rm -r '{}' \; \
      -or -name "samples" -prune -exec rm -r '{}' \; \
      -or -name "test" -prune -exec rm -r '{}' \; \
      -or -name "tests" -prune -exec rm -r '{}' \;
  cd "$pkgdir"
  patch -Np1 -i "$srcdir/upgrade.patch"

  ## atom
  cd "${srcdir}/${_pkgname}"

  _LIB="/usr/lib/${pkgname}"
  _LIBDIR="${pkgdir}/usr/lib"
  _ALIBDIR="${pkgdir}/${_LIB}"

  install -dm755 "${_LIBDIR}"
  cp -r out/Atom/resources/app ${_LIBDIR}
  mv ${_LIBDIR}/app ${_ALIBDIR}

  install -Dm755 "resources/app-icons/stable/png/1024.png" "${pkgdir}/usr/share/icons/atom.png"

  install -dm755 "${pkgdir}/usr/share/applications"
  install -Dm755 "$srcdir/${pkgname}.desktop" \
          "${pkgdir}/usr/share/applications/${pkgname}.desktop"

  install -Dm755 "$srcdir/atom.sh" "${pkgdir}/usr/bin/${pkgname}"

  install -Dm755 "out/Atom/resources/LICENSE.md" \
          "${pkgdir}/usr/share/licenses/${pkgname}/atom"

  install -Dm755 "${srcdir}/about-view.js" "${_ALIBDIR}/node_modules/about-arch/lib/about-view.js"

  # Remove useless stuff
  find "${_ALIBDIR}/node_modules" \
      -name "*.a" -exec rm '{}' \; \
      -or -name "*.bat" -exec rm '{}' \; \
      -or -name "benchmark" -prune -exec rm -r '{}' \; \
      -or -name "doc" -prune -exec rm -r '{}' \; \
      -or -name "html" -prune -exec rm -r '{}' \; \
      -or -name "man" -prune -exec rm -r '{}' \; \
      -or -path "*/less/gradle" -prune -exec rm -r '{}' \; \
      -or -path "*/task-lists/src" -prune -exec rm -r '{}' \; \
      -or -name "package.json" -exec sed -i -e "s|$srcdir|${_LIB}|g" '{}' +

  rm -rf "${pkgdir}/usr/etc"
}
