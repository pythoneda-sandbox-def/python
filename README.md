# pythoneda-sandbox/python

Definition of <https://github.com/pythoneda-sandbox/python>.

## How to declare it in your flake

Check the latest tag of this repository and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-sandbox-python = {
      [optional follows]
      url =
        "github:pythoneda-sandbox-def/python/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-sandbox-python-python38` 
- `#packages.[system].pythoneda-sandbox-python-python39` 
- `#packages.[system].pythoneda-sandbox-python-python310` 
- `#packages.[system].pythoneda-sandbox-python-python311` 
