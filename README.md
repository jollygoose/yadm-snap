This is a snap package of [yadm](https://github.com/TheLocehiliosan/yadm), an awesome dotfiles manager created by @TheLocehiliosan. 

This snap is for practice and learning purposes.

## Current disadvantages of the snap

* No man pages ([discussion](https://forum.snapcraft.io/t/support-for-man-pages/2299/22))
* No completions

---

## Creating the snap

### Requirements

* [snapcraft](https://snapcraft.io/snapcraft) (```snap install snapcraft --classic```)
* [multipass](https://snapcraft.io/multipass) (```snap install multipass```)

### Notes

The ```--classic``` flag is required in order for yadm to create and manage its directories in ```$HOME```.


### Build

```sh
git clone https://github.com/jollygoose/yadm-snap
cd yadm-snap

snapcraft

# where [current-version] is the latest version/release of yadm use the in snapcraft.yaml file.
# The --dangerous is used since this snap was built locally and does not originate from the snap store
snap install yadm_[current-version]_all.snap --classic --dangerous
```
