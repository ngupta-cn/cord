default: book

build:
	ln -s ../platform-install/docs platform-install; \
	ln -s ../../test/cord-tester/docs test; \
	ln -s ../../orchestration/xos/docs xos; \
	ln -s ../../orchestration/xos-gui/docs xos-gui; \
	ln -s ../../orchestration/profiles profiles; \
	gitbook init; gitbook install; gitbook build

book: build
	gitbook serve &
clean:
	rm -rf _book; \
	rm -rf node_modules; \
	rm platform-install; \
	rm test; \
	rm profiles; \
	rm xos; \
	rm xos-gui


