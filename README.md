This is a simple bash script to install Go. detect the version you need and then install it without any fuss

How It Works

    Architecture Detection:
        The script uses uname -m to detect the system architecture (armv6l, armv7l, or aarch64).
        It automatically selects the correct Go tarball for your Raspberry Pi model.

    Installation Steps:
        Downloads the appropriate Go version for your architecture.
        Removes any existing Go installation.
        Extracts Go to /usr/local/go.
        Adds Go's binary paths to your shell's profile (~/.bashrc).

    Verification:
        The script verifies the installation by running go version.

    Cleanup:
        The script removes the downloaded tarball after installation.

How to Use

    Copy and Save the Script: Save the script as install_go.sh.

    Make the Script Executable:

chmod +x install_go.sh

Run the Script:

    ./install_go.sh

Verification

After running the script, verify that Go is installed correctly:

    go version
