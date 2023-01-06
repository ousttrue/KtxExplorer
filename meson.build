project('KtxExplorer', 'cpp',
    version: '0.1.0',
)

imgui_dep = dependency('imgui')
ktx_dep = dependency('ktx')

executable('KtxExplorer', [
    'src/main.cpp'
],
    install: true,
    dependencies: [imgui_dep, ktx_dep],
)
