import click
import os
import subprocess

def _walk_dir(dir):
    for filename in os.listdir(dir):
        f = os.path.join(dir, filename)
        if os.path.isdir(f):  
            if filename == '.git':  
                return True
    return False

def _run_git_commands(dir):
    subprocess.run(['git','pull'])
    subprocess.run(['git','push'])
    subprocess.run(['git','push','--tags'])


@click.command()
@click.option('-d', '--dir', default='.', type=str, help='Target directory')
def run(dir):
    is_git = _walk_dir(dir)
    if is_git:
        _run_git_commands(dir)

if __name__ == '__main__':
    run()
